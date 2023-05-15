# splunk systemd unit

1. `splunk.service`

```
[Unit]
Description=Splunk
Requires=splunk-license.service
After=syslog.target network.target splunk-license.service

[Service]
Type=forking
ExecStart=/opt/splunk/splunk/bin/splunk start
ExecStop=/opt/splunk/splunk/bin/splunk stop
Restart=always

[Install]
WantedBy=multi-user.target
```

2. `splunk-license.service`

```
[Unit]
Description=Splunk licence server
After=network.target

[Service]
Type=simple
WorkingDirectory=/opt/splunk/
ExecStart=/opt/splunk/dvt-splunk_licsrv.1.0.linux.amd64
Restart=on-failure

[Install]
WantedBy=multi-user.target
```

Tags:
```
#splunk #systemd 
```
