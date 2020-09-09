# calico-k3s

[Kustomize](https://kustomize.io/) patch to install [Calico](https://www.projectcalico.org/) on [k3s](https://k3s.io/)

```
curl -sfL https://get.k3s.io | INSTALL_K3S_EXEC="--flannel-backend=none --cluster-cidr=192.168.0.0/16" sh -s -
kubectl apply -k github.com/wilsonianb/calico-k3s
```

See related issues:
- https://github.com/rancher/k3s/issues/201
- https://github.com/rancher/k3s/issues/54
