# 09-ingress

```
kubectl apply -f ingress.yaml
```

```
kubectl delete -f ingress.yaml
```

```
kubectl port-forward service/podinfo-service --namespace 09-ingress 8080:80
```

_An Ingress Controller is missing to serve request. Try opening http://localhost:80_
