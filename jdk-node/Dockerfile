FROM openjdk:8-jdk

MAINTAINER Filiosoft, LLC <Team@Filiosoft.com>

ENV NODE_VERSION 6

RUN curl -sL https://deb.nodesource.com/setup_${NODE_VERSION}.x | bash - && \
    curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && \
    apt-get install --no-install-recommends -y nodejs yarn  && \
    apt-get -y autoremove && \
    apt-get -y autoclean && \
    rm -rf /var/lib/apt/lists/* 
