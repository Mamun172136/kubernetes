###  create deployment
```bash
kubectl create deployment nginx-deployment --image=nginx:latest --replicas=3 --port=80
```
### view deployment replicaset pod
```bash
kubectl get deployment
kubectl get replicasets
kubectl get pods
```

### scale up
```bash
kubectl scale deployment nginx-deployment --replicas=7
```
### view
```bash
kubectl get deployment
kubectl get replicasets
kubectl get pods
```
### scale down
```bash
kubectl scale deployment nginx-deployment --replicas=3
```