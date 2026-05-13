### crete pod
```bash
kubectl apply -f my-pod.yaml
```
### verify pod
```bash
kubectl get pods
```
### executing command in pod
```bash
kubectl exec -it my-nginx -- /bin/bash
nginx -v
exit
```