# mysql add user
```mysql
CREATE DATABASE DB_NAME CHARACTER SET utf8 COLLATE utf8_general_ci;
CREATE USER 'DB_USER'@'%' IDENTIFIED BY 'PASSWORD';
ALTER USER 'DB_USER'@'%' IDENTIFIED WITH mysql_native_password BY 'PASSWORD';
GRANT ALL PRIVILEGES ON DB_NAME.* TO 'DB_USER'@'%';
FLUSH PRIVILEGES;
```

Tags:
```
#mysql #create_user #create_db
```

Related:
```
* Mohammad shahabi :)
```
