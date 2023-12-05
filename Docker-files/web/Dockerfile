# Use the official Nginx image as the base image
FROM nginx:latest

LABEL "Author"="Rahul Singh"
LABEL "Project"="Vprofileapp"

# Copy custom Nginx configuration file
RUN rm -rf /etc/nginx/conf.d/default.conf
COPY nginvproapp.conf /etc/nginx/conf.d/vproapp.conf

# Copy your web application files to the default Nginx public directory
COPY ./your-web-app /usr/share/nginx/html

# Expose port 80 for incoming HTTP traffic
EXPOSE 80

# Start Nginx in the foreground when the container starts
CMD ["nginx", "-g", "daemon off;"]
