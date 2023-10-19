# KubeStellar Helm Repository

Hello world!  I'm a Helm repository for KubeStellar charts.  We currently support v0.8.0 and newer versions of our KubeStellar Core components.

## Get started

Add this repository to Helm.

```
helm repo add kubestellar https://helm.kubestellar.io
```

Remember to update your local copy of our repo if its been a while since you have used it
```
helm repo update
```

## Deploy KubeStellar Core

For OpenShift
```
oc create ns kubestellar
helm install kubestellar-core kubestellar/kubestellar-core --set clusterType=OpenShift --namespace=kubestellar
```

For Kind and other Kubernetes distributions
```
kubectl create ns kubestellar
helm install kubestellar-core kubestellar/kubestellar-core --namespace=kubestellar
```

## For more information on how to use [KubeStellar's Helm chart](https://github.com/kubestellar/kubestellar/tree/main/core-helm-chart)
