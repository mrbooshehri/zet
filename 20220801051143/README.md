# Static IP address vmware NAT mode:

For static IP settings with NAT networking use an IP address between
192.168.xxx.3 and 192.168.xxx.127 (192.168.xxx.128 and above are used by
DHCP), the subnet mask 255.255.255.0 and set the Gateway 192.168.xxx.1
and DNS-Server IP addresses to 192.168.xxx.2.

Then put 8.8.8.8 in your ```/etc/resolve.conf```

Tags:
```
#vmware #static_ip #NAT
```

Related:
```
* https://communities.vmware.com/t5/VMware-Workstation-Pro/Lose-internet-connection-when-I-set-static-IP/td-p/1815112
```
