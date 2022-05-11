# Run command on Zabbix agent as root

1. Put ```sudo``` at the first of your command in ```zabbix_agent.conf``` like bellow:
```bash
UserParameter=<key>, sudo <command>
```
2. In ```/etc/sudoers``` add the following line:
```bash
zabbix  ALL=NOPASSWD: my_command
```

**Note:** replace your command with ```my_command```

Tags:
```
#Zabbix #root_agent
```

Related:
```
* https://www.zabbix.com/forum/zabbix-help/25539-user-permissions-for-userparameter
```
