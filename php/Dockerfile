FROM php:8.1.2-fpm-alpine

COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN docker-php-ext-install mysqli pdo pdo_mysql
RUN docker-php-ext-install mysqli

RUN apk add --update nodejs npm
RUN apk add --update npm

# WORKDIR /var/www/html/

# RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli

# RUN apk update && apk add npm && apk add curl 

# RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer

# RUN chmod +x /usr/bin/composer


# WORKDIR /var/www/html/

# RUN npm install && npm run dev && - php artisan migrate:fresh —seed