# Docker-Bower
Bower Docker Image for e.g. GitLab CI Runners.

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/bower.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/bower/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/bower:latest.svg)](https://imagelayers.io/?images=filiosoft/bower:latest)

----
### Pull from Docker Hub
```
docker pull filiosoft/bower:latest
```

### Build from GitHub
```
docker build -t filiosoft/bower github.com/filiosoft/dockerfiles:bower
```

### Run image
```
docker run -it filiosoft/bower bash
```

### Use as base image
```Dockerfile
FROM filiosoft/bower:latest
```