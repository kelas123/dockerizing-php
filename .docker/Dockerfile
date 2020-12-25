FROM php:7.4-fpm

RUN apt-get update && apt-get install -y \
    libfreetype6-dev \
    libjpeg62-turbo-dev \
    libpng-dev \
    libzip-dev \
    zip \
    wget

RUN groupmod -o -g 1000 www-data && \
    usermod -o -u 1000 -g www-data www-data


CMD ["php-fpm"]
EXPOSE 9000