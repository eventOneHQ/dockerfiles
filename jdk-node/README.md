# JDK with Node.js
Java JDK 8 with Node.js 8 Image for e.g. GitLab CI Runners.

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/jdk-node.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/jdk-node/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/jdk-node:latest.svg)](https://imagelayers.io/?images=filiosoft/jdk-node:latest)

### based on [openjdk:8-jdk](https://hub.docker.com/_/openjdk/)
----
### Pull from Docker Hub
```
docker pull filiosoft/jdk-node:latest
```

### Build from GitHub
```
docker build -t filiosoft/jdk-node https://raw.githubusercontent.com/Filiosoft/dockerfiles/master/jdk-node/Dockerfile
```

### Run image
```
docker run -it filiosoft/jdk-node bash
```

### Use as base image
```Dockerfile
FROM filiosoft/jdk-node:latest
```