FROM php:7.2.7-fpm-alpine3.7

RUN apk update; \
    apk upgrade;

# RUN docker-php-ext-install pdo pdo_mysql
# RUN docker-php-ext-install mysqli
RUN apk update --no-cache \
    && apk add --no-cache $PHPIZE_DEPS \
    && apk add --no-cache mysql-dev \
    && docker-php-ext-install pdo pdo_mysql
