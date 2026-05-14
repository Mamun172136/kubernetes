### Apply deployment
```bash
kubectl create -f deployment-definition.yaml
```
### imperative approach
```bash
kubectl create deployment nginx-deployment --image=nginx:latest --replicas=3 --port=80
```
### verify pod
```bash
kubectl get deployments
kubectl get pods
kubectl delete deployments nginx-deployment
```