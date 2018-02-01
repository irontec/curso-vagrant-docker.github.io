## Dockerfile

Ejemplo: PHP + Apache con mod rewrite habilitado

```CoffeeScript
FROM php:7.0-apache
RUN a2enmod rewrite
COPY ./ /var/www/html/


```

