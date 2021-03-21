# Ejercicio 6

Utilizando docker compose generar una configuración para correr dos instancias
de passwordapi (utilizando la imagen generada previamente) balanceadas por
Nginx.
La aplicación tiene un endpoint /health que indica la ip/host de la instancia
que atendió el pedido, se puede usar esto para verificar el correcto balanceo.


```
docker-compose up --scale passwordapi=2
```

Luego nos podemos dirigir a `http://localhost:4000/health`

## NOTAS

Utilicé mi propia imagen de PasswordApi [docker-hub link](https://hub.docker.com/r/apernin/passwordapi-js) basada en el código de [nicopaez/passwordapi](https://github.com/nicopaez/passwordapi)
