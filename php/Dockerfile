FROM php:7.2.1-fpm
RUN groupadd www && useradd -g www -s /sbin/nologin www
COPY php.ini /usr/local/etc/php/php.ini
COPY php-fpm.conf /usr/local/etc/php-fpm.conf
COPY php-fpm.d/www.conf /usr/local/etc/php-fpm.d/www.conf
RUN docker-php-ext-install bcmath
ADD composer.phar /usr/local/bin/composer
RUN chmod 755 /usr/local/bin/composer
VOLUME /var/www/

