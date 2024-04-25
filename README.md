
```bash
kind create cluster -n dks 
k8s config get-contexts 
k8s config use-context kind-dks
helm install dks .
```
```yaml
NAME: dks
LAST DEPLOYED: Thu Apr 25 10:20:27 2024
NAMESPACE: default
STATUS: deployed
REVISION: 1
TEST SUITE: None
NOTES:
DevOps Bootcamp: Anything in this notes file will be displayed when installing this Helm chart

1. Once you have all three pods running successfully you will need to run the following commands:
kubectl port-forward svc/frontend 3000:3000
kubectl port-forward svc/backend 8080:8080

You can access your website by navigating to:
http://localhost:3000
```