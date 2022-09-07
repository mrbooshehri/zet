# Change docker swarm node role

You can promote or demote docker swarm nodes
1. List all available nodes
```bash
docker node ls
```
2. To promote to manager
```bash
docker node promote <node_name>
```
2. To demote to manager
```bash
docker node demote <node_name>
```

Tag:
```
#docker #swarm #manager #worker #promote #demote
```

Related:
```
* https://docs.docker.com/engine/swarm/manage-nodes/
```
