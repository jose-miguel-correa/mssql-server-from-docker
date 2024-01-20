Get docker image:
```
docker pull mcr.microsoft.com/mssql/server
```
Run image locally:
```
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=<your_password>' -p 1433:1433 --name sql_server_container -d mcr.microsoft.com/mssql/server
```
Publicly expose port:
```
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=<your_password>' -p 0.0.0.0:1433:1433 --name sql_server_container -d mcr.microsoft.com/mssql/server
```


