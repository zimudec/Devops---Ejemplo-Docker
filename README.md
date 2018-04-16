# Ejemplo básico de Node con Docker
Ejemplo de un pequeño sistema en node, que se encapsula en un contenedor docker, y se levanta desde ahí.

## Prerequisitos
- [Nodejs](http://nodejs.org/en/download)
- [Docker](https://www.docker.com/get-docker)

## Uso
- Habilitar servicio de docker en tu equipo.
- Posicionarse dentro de la carpeta del proyecto y ejecutar:
```sh
#Para ejecutar lo definido en el archivo Dockerfile
$ (sudo, si es necesario) docker build -t test1 .

#Para iniciar el contenedor docker en segundo plano, con el sistema
$ (sudo, si es necesario) docker run -d -p 3000:3000 test1

#Para realizar los test
$ (sudo, si es necesario) docker run test1 npm test
```
- Entrar a través del navegador a: **[http://localhost:3000](http://localhost:3000)**

## Comandos útiles:
```sh
#Para ver contenedores iniciados
$ (sudo, si es necesario) docker ps

#Para botar contenedor
$ (sudo, si es necesario) docker kill [código]
```
