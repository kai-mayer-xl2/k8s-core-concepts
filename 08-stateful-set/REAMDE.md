# 08-stateful-set

```
kubectl apply -f stateful-set.yaml
```

```
kubectl delete -f stateful-set.yaml
```

_In a stateful set, a pod get assigned the previous volume. Try destroying the first pod and changing the replica count._