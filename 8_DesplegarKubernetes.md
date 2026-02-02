# Desplegar aplicaciones en KUBERNETES

**Nota:** Jenkins es una aplicacion que nos permite automatizar procesos.

### Imaginemos que hemos hecho algun cambio en nuestra aplicacion y queremos desplegar esta, ejecutamos el siguiente comando
```
kubectl apply -f web-php-deployment.yaml
```
### Ya hemos desplegado el deployment, ahora validamos el pod que se ha creado

```
kubectl get pods
```

### Identicamos el que se haya creado y le hacemos un describe

```
kubectl describe wev-service-etc
```

### Nos mostrara la IP, esta es la ruta por la cual podemos acceder, hacemos un curl a esa ip para validar conexion

```
kubectl curl 10.1.6.116
```

### Tiene solo una replica, modificaremos el archivo para que tenga mas replicas, modifcamos el yaml y aplicamos el cambio

```
kubectl apply -f web-php-deployment.yaml
```

### Hacemos get pods nuevamente para verlos, ya deben haber dos, luego los borramos pero se vuelven a crear por el deployment

```
kubectl get pods
kubectl delete pod wev-service-etc
```

### Obtenemos los deplyments, nos saldra el nuestro, luego lo destruiremos

```
kubectl get deploy
kubectl delete deploy wev-service-etc
```


