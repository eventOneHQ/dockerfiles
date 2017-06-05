# Node.js with rsync
Node.js 6 with rsync Image for e.g. GitLab CI Runners.

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/node-rsync.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/node-rsync/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/node-rsync:latest.svg)](https://imagelayers.io/?images=filiosoft/node-rsync:latest)

### based on [node:7](https://hub.docker.com/r/_/node/)
----
### Pull from Docker Hub
```
docker pull filiosoft/node-rsync:latest
```

### Build from GitHub
```
docker build -t filiosoft/node-rsync https://raw.githubusercontent.com/Filiosoft/dockerfiles/master/node-rsync/Dockerfile
```

### Run image
```
docker run -it filiosoft/node-rsync bash
```

### Use as base image
```Dockerfile
FROM filiosoft/node-rsync:latest
```