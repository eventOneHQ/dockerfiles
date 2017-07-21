FROM openjdk:8-jdk

MAINTAINER Filiosoft, LLC <Team@Filiosoft.com>

ENV NODE_VERSION 8

RUN apt-get update && \
    apt-get install --no-install-recommends -y apt-transport-https  && \
    curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - && \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list && \
    curl -sL https://deb.nodesource.com/setup_${NODE_VERSION}.x | bash - && \
    apt-get install --no-install-recommends -y nodejs yarn  && \
    apt-get -y autoremove && \
    apt-get -y autoclean && \
    rm -rf /var/lib/apt/lists/* 
