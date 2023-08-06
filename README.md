# itom-helm-charts

## How to use ServiceNow ITOM Helm repository

You need to add this repository to your Helm repositories:

```
helm repo add servicenow-itom https://talkapon.github.io/itom-helm-charts/
helm repo update
```

To install the K8s informer
```
helm install -n <YOUR CHOSEN NAMESPACE> --set instance.name=<YOUR INSTANCE NAME> --set clusterName="<YOUR CLUSTER NAME>" k8s-informer servicenow-itom/k8s-informer-chart
```
