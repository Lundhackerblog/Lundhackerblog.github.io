---
title: Docker Compose
type: docs
prev: docs/CERTIFICACIONES/
---

## Docker Compose

Herramienta para definir y ejecutar aplicaciones Docker multi-contenedor.

### Descripción

Docker Compose permite definir servicios, redes y volúmenes en un archivo YAML, facilitando el despliegue de aplicaciones complejas.

### Conceptos clave

- Servicios multi-contenedor
- Archivo docker-compose.yml
- Variables de entorno
- Redes personalizadas
- Volúmenes compartidos
- Escalado de servicios

### Comandos principales

- `docker-compose up`: Crear e iniciar contenedores
- `docker-compose down`: Parar y eliminar contenedores
- `docker-compose scale`: Escalar servicios
- `docker-compose logs`: Ver logs de servicios
- `docker-compose exec`: Ejecutar comandos en contenedores

### Estructura de docker-compose.yml

```yaml
version: '3.8'
services:
  web:
    image: nginx
    ports:
      - "80:80"
  database:
    image: postgres
    environment:
      POSTGRES_PASSWORD: secret
```

### Casos de uso comunes

- Aplicaciones web con base de datos
- Microservicios
- Entornos de desarrollo
- Testing automatizado
- CI/CD pipelines

### Redes en Compose

- Bridge networks por defecto
- Custom networks
- External networks
- Network aliases

## Preguntas frecuentes

*Próximamente se añadirán preguntas de práctica sobre Docker Compose.*
