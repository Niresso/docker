FROM php:8.1.1-fpm-alpine

RUN apk update && \
    apk upgrade && \
    apk add nano --upgrade make bash openssl openssl-dev libjpeg-turbo-dev libwebp-dev \
    zlib-dev libxpm-dev libpng libpng-dev icu-dev libzip-dev

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN docker-php-ext-install zip
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-install gd
RUN docker-php-ext-install intl
RUN docker-php-ext-install sockets
RUN docker-php-ext-install pcntl
RUN docker-php-ext-install bcmath
RUN docker-php-ext-install ctype
RUN docker-php-ext-install fileinfo