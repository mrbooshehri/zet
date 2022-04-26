# Zabbix tips

1. logs are under ```/var/log/zabbix/```, both server and agent
1. You can solve mariadb version problem by,
	 ```AllowUnsopportedDatabase=1``` under
	 ```/etc/zabbix/zabbix_server.conf```
