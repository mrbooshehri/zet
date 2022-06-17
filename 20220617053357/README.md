# Hot to connect to fortigate without forticlient
* Install ```openfortivpn``` package
```bash
sudo pacman -S openfortivpn
```
* Put your connection information under ```/etc/openfortivpn/conf```
	like below
```bash
### configuration file for openfortivpn, see man openfortivpn(1) ###

host = vpn.example.org
port = 443
username = vpnuser
password = VPNpassw0rd
trusted-cert = YOUR_CERT
```

Tags:
```
#Linux #forticlient #vpn
```

Related:
```
* https://github.com/adrienverge/openfortivpn
```
