# 04-replica-set

```
kubectl apply -f config-map.yaml
```

```
kubectl delete -f config-map.yaml
```

_The config map is readonly, try appending something to `/podinfo/hello.txt`_

```
echo "happy coding!" > /podinfo/hello.txt
```
