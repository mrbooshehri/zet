# Send HAProxy messages to a dedicated logfile

$AddUnixListenSocket /var/lib/haproxy/dev/log

:programname, startswith, "haproxy" {
  /var/log/haproxy.log
  stop
}

Tags:
```
#haproxy #syslog
```
