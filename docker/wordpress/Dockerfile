FROM wordpress:5.0.3-php7.1-apache

RUN apt-get update && \
	apt-get install -y  --no-install-recommends ssl-cert && \
	rm -r /var/lib/apt/lists/* && \
	a2enmod ssl && \
	a2ensite default-ssl && \
        pecl install xdebug-2.5.0 && \
        docker-php-ext-enable xdebug

EXPOSE 80
EXPOSE 443