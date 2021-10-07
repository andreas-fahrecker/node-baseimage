FROM ghcr.io/siwatinc/siwat-ubuntubaseimage:focal
RUN apt-get -y update
RUN apt-get install -y g++ gcc make ca-certificates
RUN update-ca-certificates
RUN curl -sSL https://deb.nodesource.com/gpgkey/nodesource.gpg.key | sudo apt-key add - 
RUN echo "deb https://deb.nodesource.com/node_16.x focal main" | sudo tee /etc/apt/sources.list.d/nodesource.list 
RUN apt-get install -f -y
RUN apt-get update
RUN aptitude -y install nodejs npm
RUN (mkdir -p /.npm | :) && chmod -Rv 777 /.npm
