# Docker-Fastlane
Fastlane Docker Image for e.g. GitLab CI Runners.

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/fastlane.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/fastlane/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/fastlane:latest.svg)](https://imagelayers.io/?images=filiosoft/fastlane:latest)

----
### Pull from Docker Hub
```
docker pull filiosoft/fastlane:latest
```

### Build from GitHub
```
docker build -t filiosoft/fastlane github.com/filiosoft/dockerfiles:fastlane
```

### Run image
```
docker run -it filiosoft/fastlane bash
```

### Use as base image
```Dockerfile
FROM filiosoft/fastlane:latest
```