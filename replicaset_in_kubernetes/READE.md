### apply this 
```bash
kubectl apply -f replicaset.yaml
```
### verify replicaset
```bash
kubectl get replicasets
kubectl get pods --selector=app=nginx
```
### delete pods checking self healing
```bash
kubectl delete pods --all
```
### check pod again
```bash
kubectl get pods
```