# How to disable systemd-resolved in Ubuntu

## Stages

- Disable and stop the systemd-resolved service:
```bash
		sudo systemctl disable systemd-resolved.service
		sudo systemctl stop systemd-resolved
```
- Then put the following line in the `[main]` section of your `/etc/NetworkManager/NetworkManager.conf`:
```bash
		dns=default
```
- Delete the symlink `/etc/resolv.conf`
```
		rm /etc/resolv.conf
```
- Restart network-manager
```bash
		sudo service network-manager restart
```
		or
```bash
		sudo systemctl restart NetworkManager.service
```
Tags: 
```
#Linux #systemd #resolv #systemd_resolv
```

Relates:
```
* https://askubuntu.com/questions/907246/how-to-disable-systemd-resolved-in-ubuntu
```
