FROM nginx:latest

MAINTAINER shariq

COPY index.html /usr/share/nginx/html/

EXPOSE 80

RUN apt-get update
RUN apt-get install -y git

ADD Readme /home/Readme

#set the default directory for when the container starts
WORKDIR /home
