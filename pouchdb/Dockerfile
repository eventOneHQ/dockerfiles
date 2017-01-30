FROM node:6.9-slim

RUN apt-get -qq update && \
    apt-get -y --no-install-recommends install g++ python make git wget && \
    npm install -g pouchdb-server && \
    apt-get -y purge g++ make python git && \
    apt-get -y autoremove && \
    apt-get -y autoclean

RUN mkdir /pouchdb

WORKDIR /pouchdb

CMD ["pouchdb-server", "-p", "5984", "-o", "0.0.0.0"]