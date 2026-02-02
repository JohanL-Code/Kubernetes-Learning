# Etiquetas y selectores

## Los objetos o componenetes tienen esta etiqueta, los pods, deployments y servicios.

### Sirven para que los componentes se encuentren entre ellos.

### Caracteristicas
- Las etiquetas son pares de clave/valor que se asocian a los objetos
- Las etiquetas permiten organizar o monitorear objetos de forma eficiente

## Etiquetas (Labels)
Las etiquetas son pares clave=valor que se asignan a recursos de Kubernetes como pods, services y deployments.

Sirven para identificar, agrupar y organizar recursos dentro del clúster.

Ejemplo:
```yaml
labels:
  app: nginx
  env: prod
```

**Resumen:**
- Labels identifican recursos
- Selectors buscan etiquetas
- Si no coinciden, los recursos no se conectan

