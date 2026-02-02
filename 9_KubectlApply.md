# KUBECTL APPLY

## ¿Como usar deployments?

### Creamos un deployment

```
kubectl create deployment deploy1 --image=nginx:1.21
```

### Guardamos y deployamos

```
kubectl apply -f deploy1.yaml
```

### Validamos, sacamos la IP o vemos que hay dentro

```
kubectl get pods
kubectl describe pod nginx
```

### Hacemos curl a la ip

```
curl 10.1.6.116
```

### Cambiamos la imagen del deployment para ocasionar un error, saldra el error ImagePullBackOff

```
kubectl apply -f deploy1.yaml
kubectl get pod
```

### La solucion es entrar al deployment y volverlo al estado normal

```
kubectl apply -f deploy1.yaml
kubectl get pod
```

### Modificaremos la imagen por una nueva

```
kubectl apply -f deploy1.yaml
kubectl get pod
```

### Hacemos curl con la IP a ping y deberua devolver pong

```
curl 10.1.6..151/ping
```

## Podemos crear un deployment directamente con un link

```
kubectl apply -f https://etc
kubectl get pod
```

