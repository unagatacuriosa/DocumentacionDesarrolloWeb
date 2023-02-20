## Conectarnos
Para ello usaremos las claves [[publica-privada#Keygen en ubuntu]]

```shell
ssh -p22123 usuario@ruta.maquina.com
```

## Copiamos la clave publica en el servidor

```shell
scp -P22123 /home/usuario/.ssh/id_rsa.pub usuario@ruta.maquina.com:/home/usuaio/.ssh/id_pu_insti.pub
```


## Mover la clave publica al fichero de autentificación
Con ello a la hora de conectarnos ya nos nos pedirá password
```shell
cat id_pu_insti.pub >> authorized_keys
```

## Creamos alias para conectarnos con más comodidad
Los alias es una abreviatura de un comando que hemos elegido
```shell
nano .bashrc
# Añadimos
# alias c="ssh -p22123 usuario@ruta.maquina.com"
```
 
## Reconectamos el archivo
Para evitar reiniciar la máquina
 ```shell
source .bashrc
```


## PHPSTROM
Tools>Deployment>Browse Remote Host

Aquí configurar todo como lo hemos echo anteriormente con sus keys publicas-privadas




Mapeo de puertos

Iniciamos un docker abrimos los puertos para web y creamos una carpeta en comun para que esten unidos el anfitrion y el docker

```shell
docker run -t -i --name web -p 8800:80 -v /home/alumno/docker:/var/www/html
```

En vez de crear run usamos compouser para crear varios contenedores

Crear volumenes e imagenes de docker cuando esten configurados


