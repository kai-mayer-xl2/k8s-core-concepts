# 04-replica-set

```
kubectl apply -f replica-set.yaml
```

```
kubectl delete -f replica-set.yaml
```

```
kubectl apply -f deployment.yaml
```

```
kubectl delete -f deployment.yaml
```

_The replicaSet ensures a specific number of pods is running. The deployment from the previous section does also create replicaSets and is able to handle updates and rollbacks. Try changing the env var and reapply the deployment_
