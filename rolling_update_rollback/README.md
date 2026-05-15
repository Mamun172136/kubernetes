### create deployment
```bash
kubectl apply -f deployment.yaml
```
### verify deployment
```bash
kubectl get deployments
kubectl get pods
```
### rolling update
```bash
kubectl set image deployment/nginx-deployment nginx=nginx:latest
```