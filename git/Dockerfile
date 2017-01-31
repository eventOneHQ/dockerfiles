FROM ubuntu:16.04
MAINTAINER Filiosoft <team@filiosoft.com>

RUN apt-get update && \
    apt-get install --no-install-recommends git -y && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    apt-get purge -y --auto-remove $buildDeps && \
    apt-get autoremove -y && \
    apt-get clean