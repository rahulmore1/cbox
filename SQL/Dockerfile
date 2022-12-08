FROM mcr.microsoft.com/mssql/server:2022-latest
EXPOSE 1433
USER root
RUN mkdir -p /var/opt/mssql/data && chown mssql /var/opt/mssql/data
RUN mkdir -p /var/opt/mssql/log && chown mssql /var/opt/mssql/log
RUN mkdir -p /var/opt/mssql/backup && chown mssql /var/opt/mssql/backup
USER mssql
CMD [ "/opt/mssql/bin/sqlservr" ]
