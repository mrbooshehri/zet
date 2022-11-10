# Download only debain-based

```bash
apt-get --download-only -o Dir::Cache="/path/to/destination/dir/" \
    -o Dir::Cache::archives="./" install package_name
```

Tags:
```
#download-only #download #apt #apt-get #deb
```

Related:
```
* https://askubuntu.com/questions/80665/how-can-i-direct-apt-get-to-download-package-and-its-dependencies-to-some-other
```
