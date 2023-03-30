## Ejecutar un documento de docker compose
Tenemos que estar en la carpeta donde tengamos ese archivo, y ese archivo lo creamos con las necesidades que tengamos para nuestro docker personalizado.
## Arrancar docker
```shell
# Si es sencillo volviendo a arrarcar este basta
docker compose up -d
```

Volver a arrancar otra version
```shell
docker compose up -d --force-recreate
```

## Parar docker
```shell
docker stop $(docker ps -a -q)
```

## Borrar docker
```shell
docker rm $(docker ps -a -q)
```

1.  `docker run`: Para crear y ejecutar un contenedor a partir de una imagen de Ubuntu:
    
    ```shell
    docker run ubuntu
    ```
    
2.  `docker build`: Para construir una imagen a partir de un archivo Dockerfile:
    
    ```shell
    docker build -t myimage .
    ```
    
3.  `docker images`: Para mostrar una lista de todas las imágenes almacenadas localmente en el host:
    
    ```shell
    docker images
    ```
    
4.  `docker ps`: Para mostrar una lista de todos los contenedores en ejecución actualmente:
    
    ```shell
    docker ps
    ```
    
5.  `docker stop`: Para detener un contenedor en ejecución:
    
    ```shell
    docker stop mycontainer
    ```
    
6.  `docker rm`: Para eliminar un contenedor:
        
    ```shell
    docker rm mycontainer
    ```
    
7.  `docker rmi`: Para eliminar una imagen:
    
    ```shell
    docker rmi myimage
    ```
    
8.  `docker exec`: Para ejecutar un comando dentro de un contenedor en ejecución:
    
    ```shell
    docker exec -it mycontainer bash
    ```
    
9.  `docker-compose`: Para definir y ejecutar aplicaciones de varios contenedores:
    
    ```shell
    docker-compose up
    ```
    
10.  `docker logs`: Para mostrar los registros (logs) generados por un contenedor:    
    ```shell
    docker logs mycontainer
    ```

