FROM php:7.4-apache

RUN apt-get update && apt-get install -y apt-transport-https
RUN docker-php-ext-install mysqli pdo_mysql
RUN apt-get install -y gnupg
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install -y nodejs
RUN curl -sS https://getcomposer.org/installer | php; mv composer.phar /usr/local/bin/composer ; mkdir /var/dev

# RUN mkdir /var/www && mkdir /var/www/html
# COPY php.ini /usr/local/etc/php/
# RUN echo "date.timezone = Asia/Tokyo" >> /usr/local/etc/php/php.ini

WORKDIR /var/www/html

CMD ["bash"]
