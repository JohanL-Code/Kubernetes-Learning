# Kubernetes-Learning
Kubernetes es un orquestador de contenedores que permite desplegar, escalar y mantener aplicaciones de manera optima, asi mismo, tiene una muy alta disponibilidad.

### Cluster:
Es un sistema que trata de administrar recursos de hadware simulando ser un solo componente, este puede tener multiples maquinas, instancias y los muestra al usuario como una sola aplicacion.
Un cluster administra recursos, y esos recursos son los nodos, los nodos tienen memoria, procesador, red y disco.

### Consideraciones: 
- Usa contenedores (Dockers y otros)
- Todo son objetos
- Todo se define con manifiestos (YAML)
- Si KUBERNETES muere, el app puede seguir funcionando
- Los servicios cloud tienen un servicio de administracion de kubernetes

### ¿Como nos comunicamos con kubernetes?
- Herramientas de terceros (Dashboards, Terraform). Terraforme te permite crear cosas aparte de kubernetes.
- HTTP/API REST
- CLI (Consola de comandos)

### ¿Donde lo desplegamos?
- Local
- En mv en la nube
- Usar los k8s como servicios que nos dan los proveedores cloud:
  - EKS
  - AKS
  - GKS
