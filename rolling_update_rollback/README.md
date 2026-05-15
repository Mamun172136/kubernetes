### create deployment
```bash
kubectl apply -f deployment.yaml
```
### verify deployment
```bash
kubectl get deployments
kubectl get pods
```
### anotate
```bash
kubectl anotate deployment nginx-deployment kubernetes.io/change-cause deployment
```

### rolling update
```bash
kubectl set image deployment/nginx-deployment nginx=nginx:latest
```

### anotate
```bash
kubectl anotate deployment nginx-deployment kubernetes.io/change-cause deployment
```


### verify update
```bash
kubectl get pods -l app=nginx -o jsonpath="{.items[*].spec.containers[*].image}"

```

### check deployment history
```bash
kubectl rollout status deployment/nginx-deployment
kubectl rollout history deployment/nginx-deployment
```

### roll back
```bash
kubectl rollout undo deployment/nginx-deployment --to-revision=1
```
### verify rollback
```bash
kubectl rollout status deployment/nginx-deployment
kubectl describe deployment nginx-deployment
```

### detail verification
```bash
kubectl get pods -l app=nginx -o jsonpath="{.items[*].spec.containers[*].image}"
```