### apply this 
```bash
kubectl apply -f replicaset.yaml
```
### verify replicaset
```bash
kubectl get replicasets
kubectl get pods --selector=app=nginx
```