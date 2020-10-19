FROM php:7.2

RUN apt-get update
RUN apt-get install -y git unzip
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /server

CMD ["php", "-S", "0.0.0.0:80", "-t", "public"]