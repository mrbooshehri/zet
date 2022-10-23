# Root password for fresh installed mysql
1. Find the password
```bash
grep "temporary password" /var/log/mysqld.log
```

2. Init database
```bash
mysql_secure_installation
```

Tags:
```
#mysql #password #temporary
```

Related:
```
* https://www.percona.com/blog/2016/05/18/where-is-the-mysql-5-7-root-password/
```
