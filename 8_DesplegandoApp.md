### Desplegando app con comandos Kubernetes

## Creando pods, deployments, servicios

```
kubectl apply -f<nombre-yaml>
kubectl get pod
kubectl describe pod <namepod>
kubectl log <namepod>
kubectl delete <namepod>
```

## Buscando pods
```
kubectl get pods
```

## Ver detalle del pod
```
kubectl describe pod service-us
```

**Info importante:** Muestra la ip, el nodo donde esta, la imagen, etc.

## Mostrando info del deployment de nuestro pod

```
kubectl describe deployment <nombre-pod>
```

**Info importante:** Muestra el namespace, los labels, replicas, etc.

## Mostrando info del servicio de nuestro pod

```
kubectl describe service service-us
```

**Info importante:** Muestra info del nodo, endspoints, etc.

## Mantando un pod

```
kubectl get pods
kubectl describe pod <service-us>
kubectl delete pod service-us
```

## Mostrando estado de pod en tiempo real

```
kubectl get pod -w
```

## Mostrando pod del container

```
kubectl log service-us
```




