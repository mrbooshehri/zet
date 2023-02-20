# Install sar debain

1. Install `sysstat`
```bash
sudo apt install sysstat
```
2. enable data collecting by change `ENABLED` value to `ture`
```bash
vim /etc/default/sysstat
```
3. restart the service
```bash
sudo service sysstat restart
```

Tags:
```
#sar #sysstat #monitor
```

Related:
```
* https://askubuntu.com/questions/839795/cannot-open-var-log-sysstat-sa20-no-such-file-or-directory
```
