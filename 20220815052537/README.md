# Remove ```pv``` and ```pvc``` kubernetes

## Remove pv

```bash
kubectl get pv | grep <criteria>
kubectl delete pv <pv-name>
```

## Remove pvc

```bash
kubectl get pvc -n <namespace>
kubectl delete pvc -n <namespace> <pv-name>
```


Tags:
```
#kubernetes #kubectl #pv #pvc
```

Related:
```
* Shahriar Nazemi :)
```
