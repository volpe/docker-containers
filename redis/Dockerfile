# DOCKER-VERSION 0.6.4

FROM ubuntu:latest

RUN        echo "deb http://archive.ubuntu.com/ubuntu precise main universe" > /etc/apt/sources.list
RUN         apt-get -y update
RUN         apt-get -y install redis-server
EXPOSE      6379
ENTRYPOINT  ["/usr/bin/redis-server"]