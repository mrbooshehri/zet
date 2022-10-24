# Kubernetes Rolling Deployment

A rolling deployment is the default deployment strategy in Kubernetes.
It replaces the existing version of pods with a new version, updating
pods slowly one by one, without cluster downtime.

The rolling update uses a readiness probe to check if a new pod is
ready, before starting to scale down pods with the old version. If there
is a problem, you can stop an update and roll it back, without stopping
the entire cluster.

To perform a rolling update, simply update the image of your pods using
kubectl set image. This will automatically trigger a rolling update.

To refine your deployment strategy, change the parameters in the
spec:strategy section of your manifest file. There are two optional
parameters—maxSurge and maxUnavailable:

* MaxSurge specifies the maximum number of pods the Deployment is
	allowed to create at one time. You can specify this as a whole number
	(e.g. 5), or as a percentage of the total required number of pods
	(e.g. 10%, always rounded up to the next whole number). If you do not
	set MaxSurge, the implicit, default value is 25%.
* MaxUnavailable specifies the maximum number of pods that are allowed
	to be unavailable during the rollout. Like MaxSurge, you can define it
	as an absolute number or a percentage.

At least one of these parameters must be larger than zero. By changing
the values of these parameters, you can define other deployment
strategies, as shown below.
