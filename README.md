# k8s core concepts

Some simple resources to show some k8s core concepts

Tools to install:

- k9s
- k3d
- kubectl
- helm
- docker

## Setup a cluster

```
k3d cluster create -p "80:80@loadbalancer" -p "443:443@loadbalancer" --k3s-arg "--disable=traefik@server:*" --k3s-arg "--disable=local-storage@server:*" local-k8s
```

## Destroy the cluster

```
k3d cluster delete local-k8s
```
