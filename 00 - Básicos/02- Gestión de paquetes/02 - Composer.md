Instalar curl
```shell
sudo apt install curl
```

Uso del curl para descargar una web
```shell
curl http://unizar.es
```

Instalar composer
```shell
curl -sS [https://getcomposer.org/installer](https://getcomposer.org/installer) -o composer-setup.php
```
```shell
sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```
```shell
sudo apt-get install php-curl
```

Para que funcione
```shell
composer install
```

Si has echo cambios volver a hacer (generar de nuevo el classmap)
```shell
composer update
```

Arrancar un servidor local laravel
```shell
php artisan serve &
```

Instalar breeze
```shell
# Primero este comando
composer require "laravel/breeze"
# Despues este otro
php artisan breeze:install
```

Para migrar:
```shell
php artisan migrate
```

