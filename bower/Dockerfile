FROM node:6

MAINTAINER Filiosoft <Team@Filiosoft.com>

ENV BOWER_VERSION 1.8.0

RUN npm i -g --unsafe-perm bower@${BOWER_VERSION}

RUN echo '{ "allow_root": true }' > /root/.bowerrc