##Configurar user y email de GIT

```shell
sudo apt-get update
sudo apt-get install git
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

## Para traer al *Working Directory* un archivo del Stading para modificarlo
Para antes de hacer el commit y has modificado archivos o quieres modificar.

```shell
# Si quieres un archivo
git rm --cached  <nombre archivo>
```

## *Commit* y comentario
Para commitear y acabar el flujo de trabajo.

```shell
# Si quieres un archivo
git commit -m "comentario"
```

## Clonar GIT
Para descargarse un repositorio GIT

```shell
# Si quieres un archivo
git clone url
```

## Subir GIT
Para descargarse un repositorio GIT

```shell
# Si quieres un archivo
git push --force origin main
```

## Bajar GIT
Para descargarse un repositorio GIT

```shell
# Si quieres un archivo
git pull origin main
```
