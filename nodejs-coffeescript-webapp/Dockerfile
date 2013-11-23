# DOCKER-VERSION 0.6.4

FROM ubuntu:latest

RUN        echo "deb http://archive.ubuntu.com/ubuntu precise main universe" > /etc/apt/sources.list
RUN        apt-get -y update
RUN        apt-get -y install wget 
RUN wget -O - http://nodejs.org/dist/v0.10.22/node-v0.10.22-linux-x64.tar.gz | tar -C /usr/local/ --strip-components=1 -zxv
RUN npm install -g coffee-script
ADD . /src
RUN cd /src; npm install

EXPOSE 3000

CMD ["coffee", "/src/server.coffee"]