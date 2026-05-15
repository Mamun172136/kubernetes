###

```bash
kubectl apply -f nginx-deployment.yaml
```

### auto scale

```bash
kubectl autoscale deployment nginx --cpu-percent=80 --min=3 --max=7
```

### verify hpa config

```bash
kubectl describe hpa nginx
kubectl get hpa

```

### delete

```bash
kubectl delete deployment nginx
```

### update deployment

```bash
kubectl apply -f nginx-deployment.yaml
```

### hpa create

```bash
kubectl apply -f nginx-hpa.yaml
```
