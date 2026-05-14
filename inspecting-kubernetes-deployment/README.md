### create deployment
```bash
kubectl create deployment my-nginx --image=nginx:1.999 --replicas=3
```
### verify deployments
```bash
kubectl get deployments
kubectl get pods
```
### investigate pod
```bash
kubectl describe pods
```
### edit deployment
```bash
kubectl get deployment my-nginx -o yaml > my-nginx-deployment.yaml
vim my-nginx-deployment.yaml
image: nginx:latest
cat my-nginx-deployment.yaml
kubectl delete deployment my-nginx
kubectl create -f my-nginx-deployment.yaml
kubectl get deployments
kubectl get pods
```
