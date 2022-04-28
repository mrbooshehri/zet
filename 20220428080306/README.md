# Enable and configure Centos network interface

## Check network status
```
nmcli d
```

## 	Solution 1: manually for static IP

1. open the network's configuration file

```bash
vim /etc/sysconfig/network-scripts/ifcfg-[network_device_name]
```
1. Put the following configurations
```
IPADDR=...
NETMASK=...
GATEWAY=...
DNS1=...
DNS2=...
ONBOOT="yes"
BOOTPROTO="static"
```

1. Restart network with systemctl

## Solution 2: manually for dhcp

Exactly as the same as the previous solution, just need to change one
line: ```BOOTPROTO="dhcp"```

## Solution 3: nmtui

just run ```nmtui``` command and configure the network interface

Tags:
```
#Linux #Centos #Configuration #Network
```

Related:
```
* <https://phoenixnap.com/kb/configure-centos-network-settings#ftoc-heading-4>
```
