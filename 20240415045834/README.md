# Add custom private range to vagrant using virtualbox as hyper-visor

1. Create `vbox` directory under `/etc`
```bash
sudo mkdir /etc/vbox
```

2. Create `networks.conf` and add the following line to it
```bash
sudo echo -e "* 192.168.50.0/24"
```
> Note: `192.168.50.0/24` is an example you can put your desire range or
> even several ranges

Tags:
```
#vagrant #ip #network #ip_rage #range
```

Related:
```
* https://stackoverflow.com/questions/70704093/the-ip-address-configured-for-the-host-only-network-is-not-within-the-allowed-ra
```
