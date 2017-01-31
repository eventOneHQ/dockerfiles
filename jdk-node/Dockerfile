FROM openjdk:8-jdk

MAINTAINER Filiosoft <Team@Filiosoft.com>

ENV NODE_VERSION 6

RUN curl -sL https://deb.nodesource.com/setup_${NODE_VERSION}.x | bash - && \
	apt-get install --no-install-recommends -y nodejs  && \
    apt-get -y autoremove && \
    apt-get -y autoclean && \
    rm -rf /var/lib/apt/lists/* 