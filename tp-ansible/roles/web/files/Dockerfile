FROM ubuntu:18.04

ENV DEBIAN_FRONTEND noninteractive


RUN apt update && \
    apt install apache2 php php-mysql -y && \
    chmod 777 /var/www/html && \
    rm /var/www/html/index.html

EXPOSE 80
EXPOSE 443

CMD apachectl -D FOREGROUND
