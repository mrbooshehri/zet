# Change docker directory

1. Stop docker.service and docker.socket
```bash
systemctl stop docker.service
systemctl stop docker.socket
```

2. Edit docker.service under `/lib/systemd/system/docker.service`
```bash
ExecStart=/usr/bin/dockerd -g /new/path/docker -H fd://
```

3. Restart systemd
```bash
systemctl daemon-reload
```

4. Create the docker path
```bash
mkdir -p /new/path/docker
```

5. Copy old docker to new location
```bash
rsync -aqxP /var/lib/docker/ /new/path/docker
```

6. Start docker
```bash
systemctl start docker.service
systemctl start docker.socket
```
	
Tags:
```
#docker #docker_location #docker_path
```

Related:
```
* https://linuxconfig.org/how-to-move-docker-s-default-var-lib-docker-to-another-directory-on-ubuntu-debian-linux
```
