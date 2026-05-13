### create initial pod
```bash
kubectl run my-nginx --image=nginx:1.26 
```
### verify pod
```bash
kubectl get pods
```
### export pod definition
```bash
kubectl get pod my-nginx -o yaml >my-new-pod.yaml
vim my-new-pod.yaml
spec:
  containers:
  - name: nginx
    image: nginx:latest

```
