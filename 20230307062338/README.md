# Replicaset vs Deployment in kubernetes

A ReplicaSet ensures that a number of Pods is created in a cluster. The
pods are called replicas and are the mechanism of availability in
Kubernetes. But changing the ReplicaSet will not take effect on existing
Pods, so it is not possible to easily change, for example, the image
version.

A deployment is a higher abstraction that manages one or more
ReplicaSets to provide a controlled rollout of a new version. When the
image version is changed in the Deployment, a new ReplicaSet for this
version will be created with initially zero replicas. Then it will be
scaled to one replica, after that is running, the old ReplicaSet will be
scaled down. (The number of newly created pods, the step size so to
speak, can be tuned.)

As long as you don't have a rollout in progress, a deployment will
result in a single replicaset with the replication factor managed by the
deployment.

Tags:
```
#kubernetes #replicaset #deployment
```

Related:
```
* https://stackoverflow.com/questions/69448131/kubernetes-whats-the-difference-between-deployment-and-replica-set
```
