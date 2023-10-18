# KubeStellar Helm Repository

Hello world!  I'm a Helm repository for KubeStellar charts.

## Get started

Add this repository to Helm.

```
helm repo add kubestellar https://helm.kubestellar.io
```

## Deploy KubeStellar Core

For OpenShift
```
helm install kubestellar-core kubestellar/kubestellar --set clusterType=OpenShift --namespace=kubestellar
```

For Kind and other Kubernetes distributions
```
helm install kubestellar-core kubestellar/kubestellar --namespace=kubestellar
```