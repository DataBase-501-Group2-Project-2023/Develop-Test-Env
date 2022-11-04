FROM node

LABEL maintainer="hoplin"
LABEL email="jhoplin7259@gmail.com"

RUN apt-get update -y
RUN apt-get upgrade -y

# Install VIM
RUN apt-get install vim -y

# Set working directory
RUN mkdir backend
WORKDIR /backend

# COPY server code
COPY . /backend 
# Install project dependencies
RUN npm i
#Set timezone to kst
RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime

RUN npm i

VOLUME [ "/backend" ]

# 3000 : Swagger API Docs
# 4000 : API
EXPOSE 3000 4000