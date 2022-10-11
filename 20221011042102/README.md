# Add proxy to apt

1. Create the following file
```bash
sudo touch /etc/apt/apt.conf
```
2. Add your proxy like the following pattern
```bash
Acquire::http::Proxy "http://USERNAME:PASSWORD@SERVER:PORT";
Acquire::https::Proxy "https://USERNAME:PASSWORD@SERVER:PORT";
```

Tags:
```
#Linux #apt #proxy #apt_proxy
```

Related:
```
* https://askubuntu.com/questions/257290/configure-proxy-for-apt
```
