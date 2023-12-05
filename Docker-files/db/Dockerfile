FROM mysql:8.0.33 as BUILD_IMAGE
LABEL "Author"="Rahul Singh"
LABEL "Project"="Vprofileapp"
ENV MYSQL_ROOT_PASSWORD="vprodpass"
ENV MYSQL_DATABASE="accounts"

COPY db_backup.sql /docker-entrypoint-initdb.d/db_backup.sql