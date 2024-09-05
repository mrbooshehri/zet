# Elasticsearch on docker

The `vm_max_map_count` kernel setting needs to be set to at least 262144 for production use. Depending on your platform:

The `vm_map_max_count` setting should be set permanently in `/etc/sysctl.conf`:

```bash
$ grep vm.max_map_count /etc/sysctl.conf
vm.max_map_count=262144
```
To apply the setting on a live system type: 

```bash
sysctl -w vm.max_map_count=262144
```
Tags:
```
#docker #elasticsearch #vm.max.map_count #docker-compose #graylog
```

Related:
```
* https://www.elastic.co/guide/en/elasticsearch/reference/5.1/docker.html#docker-cli-run-prod-mode
```
