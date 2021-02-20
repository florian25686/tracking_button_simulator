FROM php:7.4.6-fpm-alpine

RUN apk add --no-cache \
    bash \
    sed \
    ghostscript \
    imagemagick

COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN curl -sS https://get.symfony.com/cli/installer | bash
RUN mv /root/.symfony/bin/symfony /usr/local/bin/symfony

WORKDIR "/var/www"
EXPOSE 9000