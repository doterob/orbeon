FROM postgres:9-alpine

ENV POSTGRES_DB ORBEON
ENV POSTGRES_USER orbeon
ENV POSTGRES_PASSWORD password

ADD init.sql /docker-entrypoint-initdb.d/
RUN chmod 0777 /docker-entrypoint-initdb.d/init.sql
