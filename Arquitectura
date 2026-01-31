# Arquitectura de Kubernetes – Master

## 🏗️ Componentes del Control Plane

### 🔹 API Server
Es la interfaz principal de Kubernetes.  
Gestiona la comunicación entre el usuario (kubectl, APIs, dashboards) y los componentes internos del clúster.  
Todas las solicitudes y cambios de estado pasan por el API Server.

### 🔹 Scheduler
Componente encargado de asignar los pods a los nodos disponibles.  
Evalúa políticas, recursos, afinidad, tolerancias y disponibilidad para balancear la carga de trabajo del clúster.

### 🔹 Controller Manager
Administra los controladores que mantienen el estado deseado del sistema.  
Supervisa constantemente el estado actual y ejecuta acciones correctivas cuando hay diferencias con el estado esperado.

### 🔹 etcd
Base de datos distribuida tipo key-value.  
Almacena de forma persistente la información crítica del clúster, como estados, configuraciones, nodos y aplicaciones.  
Es un componente crítico para el funcionamiento de Kubernetes.
