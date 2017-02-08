FROM php:7.1.1-apache

RUN sed -i 's/DocumentRoot \/var\/www\/html/DocumentRoot \/var\/www\/webService\/www/g' /etc/apache2/sites-available/000-default.conf

RUN service apache2 restart
