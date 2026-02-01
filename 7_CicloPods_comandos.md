# 📦 Ciclo de Vida de los Pods en Kubernetes (Guía Operativa)

Un **Pod** es la unidad mínima de ejecución en Kubernetes.  
Su ciclo de vida representa los estados por los que pasa desde que es creado hasta que termina.

Este documento está enfocado en **operación real**, **debug desde terminal** y **entrevistas técnicas**.

---

## 🔄 Fases del Ciclo de Vida de un Pod

### 1️⃣ Pending
El Pod fue aceptado por el cluster, pero aún no se ha ejecutado en un nodo.

**Causas comunes:**
- No hay nodos disponibles
- Falta de CPU o memoria
- Imagen no descargada
- Problemas con volúmenes

**Diagnóstico:**
kubectl get pods
kubectl describe pod <pod-name>
kubectl top nodes

### 🔴 CrashLoopBackOff

**El contenedor falla y Kubernetes lo reinicia continuamente.**

kubectl get pods
kubectl describe pod <pod-name>
kubectl logs <pod-name> --previous

### 🔴 ImagePullBackOff / ErrImagePull

**Error al descargar la imagen del contenedor.**

kubectl describe pod <pod-name>

### 🔴 OOMKilled

**El contenedor fue terminado por exceso de memoria.**

kubectl describe pod <pod-name>
kubectl top pod <pod-name>

### 🔴 Pending por capacidad

**El Pod no puede ser programado.**

kubectl describe pod <pod-name>
kubectl top nodes

### 🔴 Readiness Probe Failed

**El Pod no recibe tráfico.**

kubectl describe pod <pod-name>
kubectl get endpoints <service-name>

```
kubectl get pods -o wide
kubectl get svc
kubectl describe svc <service-name>
kubectl get endpoints <service-name>
kubectl get pods --show-labels
kubectl exec -it <pod> -- curl http://localhost:PUERTO
```


