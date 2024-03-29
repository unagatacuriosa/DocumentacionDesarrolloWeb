## Configurar user y email de GIT
Instalar Git en Sistemas Linux

```shell
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git
```

## Clonar GIt
Sirve para clonar un repositorio de Github ya sea propio o ageno.
- Si es propio podremos hacer push en ellos (si trabajamos desde distintos ordenadores)
- Si es ageno NO podremos hacer push, solo nos servira para visualizar y actualizar.
```shell
git clone
```

## Iniciar GIT
Para iniciar un **nuevo repositorio** GIT en un proyecto ejecutar este comando en la carpeta principal del proyecto:

```shell
git init
```

## Ver Status GIT
Para ver como esta el estatus de los archivos del directorio de trabajo de tu proyecto:
- **staged** -> Los archivos que han sido modificados, pero aún no has sido confirmados.
- Los archivos que han sido agregados al control de versiones y están listos para ser confirmados para el *commit*.
- Las ramas actuales y cualquier cambio pendiente de ser fusionado en la rama actual.

```shell
git status
```

## GIT log
Para llevar un control de log de los git del proyecto con sus commit.

```shell
# Si quieres un archivo
git log
```


## Para añadir los archivos a *Staging Area*
Para pasar a la segunda fase del proceso y dejar los ficheros listos (acabados) para el commit.

```shell
# Si quieres un archivo
git add <nombre archivo>

# Si quieres todos los archivos
git add *
```

### Otras opciones de add
```shell
# Este añade todos menos los ocultos
git add *

#Para añadir todos con ocultos
git add -A
```


## Para traer al *Working Directory* un archivo del Stading para modificarlo
Para antes de hacer el commit y has modificado archivos o quieres modificar.

```shell
git rm --cached  <nombre archivo>
```

## *Commit* y comentario
Para commitear y acabar el flujo de trabajo.

```shell
git commit -m "comentario"
```

## Añadir tag a los commits
Para ponerte el tag
```shell
#v1.0.0
git tag nombre_tag
```

Para borrar tag
```shell
#v1.0.0
git tag -d nombre_tag
```

Para subir las tag
```shell
#v1.0.0
git push --tags
```

Para subir los commits con los tags
```shell
#v1.0.0
git push && git push --tags
```

Para ver los tags
```shell
# Muestra toda la lista de tags
git tag
```

## Clonar GIT
Para descargarse un repositorio GIT

```shell
git clone url
```

## Subir GIT
Para descargarse un repositorio GIT

```shell
git push --force origin main
```

## Bajar GIT
Para descargarse y comparar un repositorio GIT

```shell
git pull origin main
```

## Borrar el repositorio GIT
Para descargarse un repositorio GIT

```shell
git remote remove origin
```

## Conectar el repositorio GIT
Para descargarse un repositorio GIT

```shell
# HTTPS (Usuario y Key)
git remote add origin <ruta https://....>

# SSH (Clave publica/privada)
git remote add origin <ruta git@....>
```

## Comparación del código
Sirve para poder ver el código y te marca cuales han sido las modificaciones.
Es importante que el primero que pongamos sea el más antiguo para poder ver de forma correcta el flujo de modificación.

```shell
# Con git log puedes ver su id de commit (un chorrizo enorme de numeros)
git diff id_del_commit_masAntiguo id_del_commit_masReciente
```

## Cambiar de rama
```shell
git checkout master
```

## Comprobar ramas
```shell
git branch -a
```

## Cambiar nombre
```shell
git branch -m main
```

## Crear o mover rama

```shell
# con branch asecas ves las ramas
git branch nombre_rama
```

## Fusionar ramas
**¡IMPORTANTE!** Te pones en la rama que quieras mantener y le das merge (fusionar) la que quieras mezclar.
```bash
git merge nombre_rana
```

## Borrar rama
```shell
git branch --delete nombre_rama
```
