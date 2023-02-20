# How to add Certificate Authority file in CentOS 7

1. copy your certificates inside
```bsah
/etc/pki/ca-trust/source/anchors/
```
2.then run the following command
```bash
update-ca-trust
```

Tags:
```
#cet #ca #certificates #authority #public #key
```

Related:
```
* https://stackoverflow.com/questions/37043442/how-to-add-certificate-authority-file-in-centos-7
* https://www.redhat.com/sysadmin/configure-ca-trust-list
```
