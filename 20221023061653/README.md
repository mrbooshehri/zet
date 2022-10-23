# How could we allow non-root users to control a systemd service?

Open ```/etc/sudoers``` and add the following lines

```bash
%<username> cms051=/usr/bin/systemctl restart <service-name>.service
%<username> cms051=/usr/bin/systemctl stop <service-name>.service
%<username> cms051=/usr/bin/systemctl start <service-name>.service 
%<username> cms051=/usr/bin/systemctl status <service-name>.service
```

Tags:
```
#linux #systemd
```

Related:
```
* https://linuxsheet.com/answers/192706/
```
