# Docker-Git
Bower Git Image for e.g. GitLab CI Runners.

## WARNING: This `Dockerfile` has been moved to the Filiosoft GitLab. You can find it [here](https://developers.filiosoft.com/docker/git). 

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/git.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/git/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/git:latest.svg)](https://imagelayers.io/?images=filiosoft/git:latest)

----
### Pull from Docker Hub
```
docker pull filiosoft/git:latest
```

### Build from GitHub
```
docker build -t filiosoft/git github.com/filiosoft/dockerfiles:git
```

### Run image
```
docker run -it filiosoft/git bash
```

### Use as base image
```Dockerfile
FROM filiosoft/git:latest
```