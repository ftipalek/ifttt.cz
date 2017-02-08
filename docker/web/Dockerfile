FROM php:7.1.1-apache

#RUN openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/apache-selfsigned.key -out /etc/ssl/certs/apache-selfsigned.crt -subj "/C=CZ/ST=Brno/L=Brno/O=IFTTT.CZ/OU=IFTTT.CZ/CN=ifttt.cz"

RUN sed -i 's/DocumentRoot \/var\/www\/html/DocumentRoot \/var\/www\/webService\/www/g' /etc/apache2/sites-available/000-default.conf

#RUN sed -i 's/DocumentRoot \/var\/www\/html/DocumentRoot \/var\/www\/webService\/www/g' /etc/apache2/sites-available/default-ssl.conf
#RUN sed -i 's/\/etc\/ssl\/certs\/ssl-cert-snakeoil.pem/\/etc\/ssl\/private\/apache-selfsigned.key/g' /etc/apache2/sites-available/default-ssl.conf
#RUN sed -i 's/\/etc\/ssl\/private\/ssl-cert-snakeoil.key/\/etc\/ssl\/private\/apache-selfsigned.key/g' /etc/apache2/sites-available/default-ssl.conf

#RUN a2enmod ssl
#RUN a2ensite default-ssl.conf

RUN service apache2 restart
