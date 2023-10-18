# KubeStellar Helm Repository

Hello world!  I'm a Helm repository for KubeStellar charts.  We currently support v0.8.0 and newer versions of our KubeStellar Core components.

## Get started

Add this repository to Helm.

```
helm repo add kubestellar https://helm.kubestellar.io
```

Remember to update your local copy of our repo if its been a while since you have used it
```
helm update
```

## Deploy KubeStellar Core

For OpenShift
```
helm install kubestellar-core kubestellar/kubestellar-core --set clusterType=OpenShift --namespace=kubestellar
```

For Kind and other Kubernetes distributions
```
helm install kubestellar-core kubestellar/kubestellar-core --namespace=kubestellar
```