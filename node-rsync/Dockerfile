FROM node:7
MAINTAINER Filiosoft <Team@Filiosoft.com>

RUN apt-get -qq update && \
    apt-get -y --no-install-recommends install rsync && \
    apt-get -y autoremove && \
    apt-get -y autoclean && \
    rm -rf /var/lib/apt/lists/* 