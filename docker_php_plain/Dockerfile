FROM php:8.0-apache

LABEL maintainer="hoplin"
LABEL email="jhoplin7259@gmail.com"

RUN apt-get update -y
RUN apt-get upgrade -y

RUN apt-get install -y git
RUN apt-get install -y gcc

VOLUME [ "/var/www/html" ]
EXPOSE 80