# K8S VOLUMEN y STORAGE

## Storage
- Comportamiento por defecto
- Los pod no guardan informacion
- La info se pierde cuando el pod muere
- Los contenedores no comporten info con otro contenedor

## Tipos de Volumenes
- Se pueden defifnir tipos de volumen para cambiar el comportamiento por defecto
- Pueden cambiar dependiendo del tipo de nube donde se aloje el cluster
- No comporten disco aunque esten en el mismo nodo

## Ejemplo de tipos de volumenes
- Mismo pod compartiendo el mismo volumen
- Volumen externo a la capacidad de agregarse a un nodo a la vez
