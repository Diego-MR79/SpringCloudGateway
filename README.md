# Gateway Server

Servicio que enruta los microservicios del proyecto CapySoft.

## Docker

Construir la imágen:

```shell
docker build -t gateway-server .
```

Ejecutar contenedor:

```shell
docker run --name gateway-server --network capysoft_network -d -p 8090:8090 gateway-server
```

## Uso

Esta aplicación requiere que se este levantado el servicio de eureka-server y la base de datos mysql-server.

http://localhost:8090/api/