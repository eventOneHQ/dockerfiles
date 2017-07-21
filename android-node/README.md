# Android SDK with Node.js
Android SDK 26 with Node.js 8 Image for e.g. GitLab CI Runners.

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/android-node.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/android-node/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/android-node:latest.svg)](https://imagelayers.io/?images=filiosoft/android-node:latest)

### based on [filiosoft/jdk-node](https://hub.docker.com/r/filiosoft/jdk-node/)
----
### Pull from Docker Hub
```
docker pull filiosoft/android-node:latest
```

### Build from GitHub
```
docker build -t filiosoft/android-node https://raw.githubusercontent.com/Filiosoft/dockerfiles/master/android-node/Dockerfile
```

### Run image
```
docker run -it filiosoft/android-node bash
```

### Use as base image
```Dockerfile
FROM filiosoft/android-node:latest
```