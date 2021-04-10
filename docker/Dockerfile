FROM php:7.4-apache
LABEL maintainer="estherpeixoto13@gmail.com"

RUN apt-get update && \
	apt-get install -y \
	nano \
	git \
	curl \
	apt-utils

RUN curl -sS https://getcomposer.org/installer | php -- --version=2.0.12 --install-dir=/usr/local/bin --filename=composer

RUN a2enmod rewrite

WORKDIR /var/www/

CMD apachectl -DFOREGROUND