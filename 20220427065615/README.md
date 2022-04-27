# Keep in mind Zabbix configuration

## Server
```
DBName= `the name of your database you defined in your mariadb`
DBUser= `the user you defined in your mariadb`
DBPassword= `the password you set for db on your mariadb`
AllowUnsopportedDBVersion= `if you have db conflict and you want to
ignore it,make it 1`
```

## Agent
```
Server= `IP of the server you want to connect to. withouth any mask ex:
\24`
ListenIP= `keep it as the defualt value.`
ServerActive= `IP of the server you want to connect to. withouth any mask ex:
\24`
Hostname= `The host name you have been created in your zabbix GUI/web server`
```

Tags:
```
#Zabbix
```

Related:
```
* Shahriar
```
