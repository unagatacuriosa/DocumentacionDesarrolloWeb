# Instalar Laravel
```shell
composer global require "laravel/installer"
```

# Configurar PATH
Es importante este paso, porque no se instala en el path predefinido de programas y si lo ejecutamos sin esto el bash no lo encuentra.
```shell
# Esta en la carpeta raid
nano .bashrc (o sudo nano)  
# Añadir ->
PATH=$PATH:/home/alumno/.config/composer/vendor/laravel/installer/binActu
#actualizar .bashrc
source .bashrc
```

# Conectar al terminal en carpeta
```shell
# Para iniciar un server local de Laravel
php artisan serve &
```

## Acceder en navegador
Todo depende del puerto que se te abra.
`localhost:8001`

# Crear un controlador
```shell
 php artisan make:controller
 ```

# Comandos útiles
Iniciar proyecto nuevo Laravel
```shell
laravel new nombre
```

Ver lista de rutas
```shell
php artisan route:list
```


# Iniciar el proyecto
```shell
# Arrancar el docker con la base de datos
# localhost:8800
docker compose up -d

# Para iniciar un server local de Laravel
php artisan serve &

# Para iniciar el herramienta de transpiracion del cliente (en este caso carga el CSS)
npm run dev
```

# Sistema de carpetas
## Model
- Todo lo que tiene que ver con las tablas y que interactuen

## Vista
- resources -> views
Las paginsa html
Se tienen que nombrar siempre de la misma forma.
`nombre.blade.php`

## Controlador
- app -> Http -> Controllers
- La parte php
Aquí haras toda la parte back de la web

## Ruta
- routes
- Los distintos recursos que voy a dejar disponible en mi aplicacion
- Las cosas que solicito
- index.php / juego.php / calculara.php

## Bases de datos
- database
- Más desarolllo que para producion
- La peticiones y control de la base de datos
	- factories -> valores tabla
	- migration -> crear tabla
	- seeders -> poblar tablas

## Public
Aquí pones todo lo que quieres que se renderice publicamente en el navegador

# Fundamentos
- `{{}}` -> Dentro de doble brakets puedes poner variables php creadas en back *(controlador)* para poder usarla en el front con esta sentencia. 
```php
# Misma forma de llamar a una variable desde front
<?=$nombre?>
<?php echo $nombre;?>

# Exclusivo de Laravel
{{$nombre}}
```

- `@` -> Para usar sentencias propias de Laravel
```php
# Con este creamos el front de una web en html usando Blade (que usa laravel)
@extends("layout")  
@section("menu")  
    <a href="about">About</a>  
    <a href="contact">Contact</a>  
    <a href="news">News</a>  
@endsection  
@section("contenido")  
    <h1>Pagina principal</h1>  
@endsection
```

# Librerias
- **BREEZE** -> Gestor de autentifación

# Componentes
- Pueden contener html, css y js
- Su estructura para llamarlos es la etiqutea `<x-nombre>`
- Son etiquetas dobles así que tiene una de cierre
-  Se crean en view->components
- Si estan dentro de una carpeta la etiqueta es `<x-carpeta.nombre>`


# Variables
- Se crear en controlador
- Se llaman con `{{$nombre}}`

# Migraciones
Tenemos que crear el archivo .php que usa el comando de migraciones

```shell
php artisan make:migration Empresa --create=empresas
```

Comando de migracion que ejecuta los archivos que estan en **database -> migrations**

```shell
# Hacer la migracion
 php artisan migrate

# Hacer la migracion desde 0 (perderias los datos)
 php artisan migrate:fresh

# Hacer una nueva migracion sin borrar la anterior
 php artisan migrate --i
```

# Modelo 
**Lo primero que creamos**
Para crear un modelo de migración automatico, cosas que crea de forma automática:
- Http -> Controllers -> EmpresaController.php
- database -> factories -> EmpresaFactory.php
- database -> migrations -> create_empresas_table.php
- database -> seeders -> EmpresaSeeder.php
```shell
php artisan make:Model Empresa --all
```

