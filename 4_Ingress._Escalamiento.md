# Ingress en KUBERNETES
Son balaceadores u objetos que estan entre el servicio y el internet. El Ingress controla cómo entra el tráfico web al clúster y hacia qué servicio va.

# HPA Y VPA
Son metodos de escalamiento que se usan para poder escalar la aplicacion automaticamente, esto aumenta o disminuye segun la carga que tengan los pods.

## HPA
Escalan los pods se manera horizontal, creando y eliminando pods segun la demanda que tenga la aplicacion.

### Caracteristicas:
- Define el objeto que deseas escalar
- Define el maximo y minimo de replicas
- Define el recurso a monitorear
- Define la refla para escalar

## VPA
Es mas automtico que el HPA, este es un escalamiento vertical, es decir, aumenta la capacidad del pod segun la carga que este reciba.

### Caracteristicas:
- No agrega un pod, lo reemplaza
- El escalado es automatico
