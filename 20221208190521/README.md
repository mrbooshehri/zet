# Vagrant private network access denied

## Error message:
```
Stderr: VBoxManage: error: Code E_ACCESSDENIED (0x80070005) - Access denied (extended info not available)
```

## Fix:
1. Make ```vbox``` directory uncer ```/etc```
```bsah
sudo mkdir /etc/vbox
```
2. Add your net-id in ```networks.conf```
```bash
sudo cat > /etc/vbox/networks.conf <<EOF
* 192.168.50.0/24
EOF
```

Tags:
```
#vagrant #private_network #nat #virtualbox #vb
```

Related:
```
* https://stackoverflow.com/questions/69728426/e-accessdenied-when-creating-a-host-only-interface-on-virtualbox-via-vagrant
* https://stackoverflow.com/questions/69722254/vagrant-up-failing-for-virtualbox-provider-with-e-accessdenied-on-host-only-netw
```
