Mapeo de puertos

Iniciamos un docker abrimos los puertos para web y creamos una carpeta en comun para que esten unidos el anfitrion y el docker

```shell
docker run -t -i --name web -p 8800:80 -v /home/alumno/docker:/var/www/html
```

En vez de crear run usamos compouser para crear varios contenedores

Crear volumenes e imagenes de docker cuando esten configurados


