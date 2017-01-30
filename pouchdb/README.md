# PouchDB in Docker
[![](https://images.microbadger.com/badges/image/filiosoft/pouchdb.svg)](http://microbadger.com/images/filiosoft/pouchdb "Get your own image badge on microbadger.com")
[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/pouchdb.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/pouchdb)

[PouchDB](https://pouchdb.com/) Docker image. 

### based on [node:6.9-slim](https://hub.docker.com/_/node/)
----
### Pull from Docker Hub
```
docker pull filiosoft/pouchdb:latest
```

### Build from GitHub
```
docker build -t filiosoft/pouchdb github.com/filiosoft/dockerfiles:pouchdb
```

### Run image
```
docker run -it filiosoft/pouchdb bash
```

### Use as base image
```Dockerfile
FROM filiosoft/pouchdb:latest
```