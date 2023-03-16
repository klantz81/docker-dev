FROM php:8.2-apache

RUN apt -y update && \
    apt -y upgrade && \
    apt -y install libcurl4 libcurl4-openssl-dev zlib1g zlib1g-dev libpng-dev && \
    docker-php-ext-install curl && \
    docker-php-ext-install exif && \
    docker-php-ext-install fileinfo && \
    docker-php-ext-install gd && \
    docker-php-ext-install iconv && \
    docker-php-ext-install mysqli && \
    docker-php-ext-install opcache && \
    docker-php-ext-install pdo && \
    docker-php-ext-install pdo_mysql && \
    a2enmod rewrite headers && a2enmod ssl