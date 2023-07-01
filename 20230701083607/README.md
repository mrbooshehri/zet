# Elasticsearch useful commands

1. Under dev tools use the following commands

```
#Check Cluster
GET /_cat/health?v

#Check Tedad nodeha va clusterha
GET /_cat/nodes?v

#View Index
GET /_cat/indices?v

#Disk va vaziyat nodeha
GET /_cat/allocation?v

#vaziyat shardha
GET /_cat/shards?v

#namaye state index ha
GET /_cluster/allocation/explain?pretty

#Ram
GET /_cat/nodes?v=true&h=name,node,hea
```

Tags:
```
#elk #ELK #elasticsearch #devtools #dev #tools
```

Related:
```
* Amir Abdollahian
```
