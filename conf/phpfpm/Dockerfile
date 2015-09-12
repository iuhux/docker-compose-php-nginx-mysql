FROM php:5.6-fpm
MAINTAINER XU HUI <gw.iuhux@gmail.com>

# Install modules
#RUN apt-get update \
#    && apt-get install -y \
#    && docker-php-ext-install \
#        pdo_mysql

# PHP config
ADD ./config/php.ini    /usr/local/etc/php/php.ini
ADD ./config/php-fpm.conf    /usr/local/etc/php-fpm.conf

# Composer
#ADD composer.phar /usr/local/bin/composer
#RUN chmod 755 /usr/local/bin/composer


# WORKDIR /var/www/src

# Write Permission
# RUN usermod -u 1000 www-data


VOLUME /usr/local/etc/
VOLUME /var/www/src
CMD ["php-fpm"]
