# Upgrade centos to oracle

1. Update ```yum```
```bash
sudo yum update
```
2. Download Oracle Script to Migrate to CentOS Linux
```bash
curl -O https://raw.githubusercontent.com/oracle/centos2ol/main/centos2ol.sh
```
3. Make the script executable
```bash
chmod u+x centos2ol.sh
```
4. Change your DNS to [shecan](https://shecan.ir/)
```bash
vim /etc/resolve.conf
nameserver 185.51.200.2
````
5. Run the script
```bash
./centos2ol.sh
```

Tags:
```
#Linux #oracle #centos #centos2oracle #centos_to_oracle
```

Relatd:
```
* https://www.how2shout.com/linux/how-to-migrate-centos-linux-6-7-8-servers-to-oracle-linux/
* https://github.com/oracle/centos2ol/
```
