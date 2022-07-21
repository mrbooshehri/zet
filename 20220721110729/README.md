# Configure network adapter with ```netplan```

You can find it under one of these places:
1. ```/etc/netplan```
1. ```/lib/netplan```
1. ```/run/netplan```

If you couldn't find them run the following commmand:
```bash
sudo netplan generate
```

To add static IP address replace the following config with yours:

```yaml
network:
  version: 2
  renderer: networkd
  ethernets:
    enp0s3:
     dhcp4: no
     addresses: [192.168.1.222/24]
     gateway4: 192.168.1.1
     nameservers:
       addresses: [8.8.8.8,8.8.4.4]
```

then run the following commmand to apply changes

```bash
sudo netplan apply
```

in case of facing with problens run the previous in ```debug``` mode	

```bash
sudo netplan --debug apply
```

Tags:
```
#Linux #Ubuntu #Netplan #Network_config
```

Related:
```
* https://linuxconfig.org/how-to-configure-static-ip-address-on-ubuntu-18-04-bionic-beaver-linux
```
