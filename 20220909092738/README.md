# Docker registry mirror for Iranian users

1. Create ```daemon.josn``` under following path

```bash
vim /etc/docker/daemon.json
```

2. Add the following lines in the created file
```bash
{
    "registry-mirrors": ["https://registry.docker.ir"]
}
```

3. Restart daemon and service
```bsah
systemctl daemon-reload
systemctl restart docker
```

Tags:
```
#docker #registry #docker.ir
```

Related:
```
* http://docker.ir/
```

