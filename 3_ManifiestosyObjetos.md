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
Son controladres que maneajan pods
