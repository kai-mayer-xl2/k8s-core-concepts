# 10-helm

## Traefik

```
helm install -f traefik.values.yaml --create-namespace --namespace 10-helm traefik oci://ghcr.io/traefik/helm/traefik
```

```
helm uninstall traefik --namespace 10-helm
```

## foo-podinfo

```
helm install -f podinfo-foo.values.yaml --create-namespace --namespace 10-helm foo-podinfo oci://ghcr.io/stefanprodan/charts/podinfo
```

## bar-podinfo

```
helm install -f podinfo-bar.values.yaml --create-namespace --namespace 10-helm bar-podinfo oci://ghcr.io/stefanprodan/charts/podinfo
```

_The helm chart can also expressed as rendered template_

```
helm template -f podinfo-foo.values.yaml --create-namespace --namespace 10-helm foo-podinfo oci://ghcr.io/stefanprodan/charts/podinfo > podinfo-foo.yaml
```

_Try opening http://foo.localhost:80 or http://bar.localhost:80_
