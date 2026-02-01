# Manifiestos y objetos

## Estructura de un YAML
Es un formato legilble para los usuarios, del cual podemos hacer una consulta y nos devuelve una estructura parecida al XML.
Todos los objetos se pueden crear con un YAML.

## NameSpace
Son espacios de nombre que limita lo que puedes ver, en Kubernetes solo se te mostrara los KUBERNETES que sean parte de este NameSpace.

## Orden de los objetos
Service -> Deployment -> Pod

- El pod es el contenedor como tal.
- Un deployment tiene definido un pod, y dentro del pod n contenedores.

## Parametros configurables en un pod
- namme
- image
- commmand
- args
- ports
- volumeMounts
- livenessProbe
- readinessProbe

## Deployment
Son controladres que maneajan pods. Con esto tu puedes hacer un cambio o modificar la estructura de un pod sin que se caiga la aplicacion, asi mismo, si hay algun problema puedes volver a la version anterior.
Lo que hace el deployment es que cuando mandas algun cambio, crea un nodo para ver si todo esta bien, y el otro lo desactiva, si esta todo bien, elimina el antiguo y se queda con el nuevo. Asi mismo, define cuantas replicas de una aplicacion deben estar corriendo.

## Servicios
Son un objeto que permite que un pod se comunique con el exterior.

### Consideraciones
- Un pod tiene una IP
- Un nodo tiene una IP
- La IP de los pods no son fijos
- Los pods tienen dns unico

Los servicios agrupan pods y crean politicas de acceso.

### Tipos de servicios
- ClusterIP expone el servicio internamente
- NodePort expone el servicio al exterior en la IP de cada nodo y usa puerto estatico
- LoadBalancer expone un servicio externamente usando un balanceador de carga de proveedor de nube







