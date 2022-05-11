# Run Zabbix agent as root

1. Make a systemd unite under ```/etc/systemd/system/zabbix-agent.service.d/override.conf```

```bash
[Service]
User=root
Group=root
```

2. Change following values in ```zabbix_agent.conf``` file under ```/etc/zabbix/```
```bash
AllowRoot=1
User=root
```
3. Reload ```systemd``` and ``zabbix-agent```
```bash
systemctl daemon-reload
systemctl restart zabbix_agent
```

Tags:
```
#Zabbix #Zabbix-agent #root_access #root_agent
```

Related:
```
* https://www.zabbix.com/documentation/4.0/en/manual/appendix/install/run_agent_as_root
```
