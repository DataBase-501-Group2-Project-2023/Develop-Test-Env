FROM php

LABEL maintainer="hoplin"
LABEL email="jhoplin7259@gmail.com"

# Initiate apt-get package manager
RUN apt-get update -y
RUN apt-get upgrade -y

# Get php composer
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer

COPY . /usr/src
WORKDIR /usr/src

CMD [ "php", "index.php" ]
