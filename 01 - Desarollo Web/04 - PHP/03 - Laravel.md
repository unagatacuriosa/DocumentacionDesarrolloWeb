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

# Conectar al terminal en carpeta:
```shell
php artisan serve &
```

## Acceder en navegador
Todo depende del puerto que se te abra.
localhost:8001

# Crear un controlador
```shell
 php artisan make:controller
 ```

## Ruta del controlador
- app -> Http -> Controllers

## Ruta de la vista
- resources -> views

