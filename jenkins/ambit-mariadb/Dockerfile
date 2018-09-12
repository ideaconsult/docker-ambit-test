FROM mariadb

ADD --chown=mysql:mysql https://raw.githubusercontent.com/ideaconsult/ambit-mirror/master/ambit2-all/ambit2-db/src/main/resources/ambit2/db/sql/create_tables.sql /docker-entrypoint-initdb.d/
COPY --chown=mysql:mysql dbgrants.sql /docker-entrypoint-initdb.d/

ENV MYSQL_ROOT_PASSWORD ambit
ENV MYSQL_DATABASE ambit2
ENV MYSQL_USER guest
ENV MYSQL_PASSWORD guest

CMD ["--character-set-server=utf8mb4", "--collation-server=utf8mb4_unicode_ci"]
