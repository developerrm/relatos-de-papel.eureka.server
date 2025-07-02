## Docker
Primero debemos haber creado una red Docker con:
- `docker network create relatos-net`
### Construir la imagen
- `docker build -t eureka .`
### Ejecutar el microservicio usando Docker
- `docker run --detach --network relatos-net --publish 8761:8761 eureka`