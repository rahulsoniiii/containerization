FROM mysql:8.0.33
# Give right Password in Docker Compose File
LABEL Author="Rahul Soni"
ENV MYSQL_DATABASE="accounts"
ENV MYSQL_USER="rahul"
ENV MYSQL_PASSWORD="wrong"
ENV MYSQL_ROOT_PASSWORD="root"
ADD db_backup.sql /docker-entrypoint-initdb.d/db_backup.sql
EXPOSE 3306
CMD [ "mysqld" ]