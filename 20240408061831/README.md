# Set 403.online DNS in docker to skip 403 during docker build

```bsah
sudo cat /etc/docker/daemon.json
{
    "dns": ["10.202.10.202", "10.202.10.102"]
}
```

Tags:
```
#docker #build #docker_build #dns #403
```

Related:
```
* https://superuser.com/questions/1302921/tell-docker-to-use-the-dns-server-in-the-host-system
```
