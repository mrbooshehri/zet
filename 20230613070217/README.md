# Change docker root data path

1. Stop the docker daemon

```bsah
sudo service docker stop
```

2. Add a configuration file to tell the docker daemon what is the
	 location of the data directory

2.1. Version before v17.05.0

```bash
cat >  /etc/docker/daemon.json <<EOF
{ 
   "graph": "/path/to/your/new/docker/root" 
}
EOF
```

2.2. v17.05.0 and newer

```bash
cat >  /etc/docker/daemon.json <<EOF
{ 
   "data-root": "/path/to/your/new/docker/root" 
}
EOF
```

3. Copy the current data directory to the new one

```bash
rsync -aP /var/lib/docker/ "/path/to/your/new/docker/root"
cp -rp /var/lib/docker/* "/path/to/your/new/docker/root/"
```

4. Rename the old docker directory

```bsah
mv /var/lib/docker /var/lib/docker.old
```

5. Restart the docker daemon

```bsah
service docker start
```

6. Start the service, if it works fine remove the old data

```bash
rm -rf /var/lib/docker.old
```

Related:
```
* https://tienbm90.medium.com/how-to-change-docker-root-data-directory-89a39be1a70b
```

Tags:
```
#docker #data #root-date #/var/lib/docker
```

