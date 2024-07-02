# Install `s3cmd` on SHITTY `CentOS7`

1. Add repository
```bash
yum -y install yum-utils 
yum install \
https://repo.ius.io/ius-release-el7.rpm \
https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
```

2. Install `python`
```bash
yum -y install python36u
```

3. Install `pip`
```bash
yum -y install python36u-pip
```
4. Install `s3cmd`
```bash
pip3 install --trusted-host pypi.python.org --trusted-host=*.pypi.python.org --trusted-host=pypi.org --trusted-host=*.pypi.org s3cmd
```
5. Add `s3cmd` to path
```bash
ln -sf /usr/local/bin/s3cmd /usr/bin/s3cmd
```

Tags:
```
#s3mcd #centos7 #centos #7 #python3
```

Related:
```
* https://azdigi.com/blog/en/linux-server-en/install-python-3-and-set-it-as-the-default-on-centos-7/
```
