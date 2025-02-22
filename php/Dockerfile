# Usamos una imagen base de PHP con Apache
FROM php:7.4-apache

# Instalamos la extensión para MySQL
RUN docker-php-ext-install mysqli

# Copiamos los archivos PHP al contenedor
COPY . /var/www/html/

# Exponemos el puerto 80
EXPOSE 80
