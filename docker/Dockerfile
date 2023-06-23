FROM php:7.4-fpm

RUN apt-get update && apt-get install -y \
    libzip-dev \
    zip \
    unzip

RUN docker-php-ext-install pdo pdo_mysql mysqli zip

RUN docker-php-ext-enable pdo pdo_mysql mysqli zip

WORKDIR /var/www/html

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

RUN composer create-project --prefer-dist laravel/laravel:6.* /var/www/html

RUN chmod -R 777 /var/www/html/