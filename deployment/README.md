### Apply deployment
```bash
kubectl create -f deployment-definition.yaml
```
### imperative approach
```bash
kubectl create deployment nginx-deployment --image=nginx:latest --replicas=3 --port=80
```