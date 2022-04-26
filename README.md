Pasos a seguir para la instalación:

    1- Descomprimimos la carpeta y accedemos a ella.
    2- Ejecutamos el comando "docker-compose up -d nginx php-fpm phpmyadmin mariadb workspace".
    3- Tendremos que crear un usuario y una base de datos para moodle.
    4- Levantaremos Moodle con el comando "docker-compose up -d moodle".
    5- Cuando haya finalizado podremos acceder a Moodle con localhost desde el puerto 8082.
    6- Crearemos la aplicación Laravel con este comando: 
        "docker run -it --rm --name php-cli \
        -v "$PWD:/usr/src/app" thecodingmachine/php:7.4-v3-slim-cli \
        composer create-project --prefer-dist laravel/laravel nombreApp"
