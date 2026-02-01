# Comandos
- kubectl get
- kubectl apply
- kubectl delete
- kubectl rollout
- kubectl log
- kubectl describe

## Comandos GET
- kubectl get pod
- kubectl get deploy
- kubectl get ns
- kubectl get hpa
- kubectl get service

## kubectl get ns:
Muestra todos los nameSpace que tenga nuestro kubernetes, solo nos muestra el nombre, el tiempo y el estatus. Cada uno de estos tiene recuresos separados.

## kubectl get all:
Muestra todos los componenetes de nuestro kubernetes, pods, deplyments, replicaset, hpa.

## kubectl get node:
Son la maquina donde estan nuestros pods, mustra la informacion de los nodos.

## kucectl get pod:
Obtiene el estado de los nodos

## kubectl get deploy:
Se deben nodos en base a deployments, tambien controla las replicas entre otros, da una lista de las replicas y cuantas de estas estan funcionando.

## kubectl get service:
Son componenetes que permiten publicar o hacer esa salida hacia internet, permite que los pods se encuentren y comuniquen de manera confiable.
Un servicio esta asociado a un deployment, y este ultimo a los pods

## kubectl replicaset:
Ver a lista de los replicaset

## kubectl HPA:
Son recursos que me permiten ver el escalado de la aplicacion, si mis pods estan saturados, segun la regla se vuelve a crear otro pod.

## kubectl top pod:
Es un comando que muestra mas info a nivel de recursos a nivel de pods y nodos.















