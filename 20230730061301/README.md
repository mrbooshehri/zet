# Log filter rsyslog

1. Create a confing file under `/etc/rsyslog.d`

```bash
vim /etc/rsyslog.d/example.conf
```

2. Add your conditions like the following

```bash
if $programname contains "bash" then {
	action(type="omfwd" target="{{graylog_server}}" port="{{graylog_port}}" protocol="{{graylog_portocol}}")
}
if $msg contains_i "session" then {
	action(type="omfwd" target="{{graylog_server}}" port="{{graylog_port}}" protocol="{{graylog_portocol}}")
}
```

3. restart rsyslog

Tags:
```
#rsyslog #linux #log_filter #log #filter
```
