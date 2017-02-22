# rsync in Docker
[![](https://images.microbadger.com/badges/image/filiosoft/rsync.svg)](http://microbadger.com/images/filiosoft/rsync "Get your own image badge on microbadger.com")
[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/rsync.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/rsync)

`rsync` Docker image. 

### based on [alpine:3.3](https://hub.docker.com/_/alpine/)
----
### Pull from Docker Hub
```
docker pull filiosoft/rsync:latest
```

### Build from GitHub
```
docker build -t filiosoft/rsync github.com/filiosoft/dockerfiles:rsync
```

### Run image
```
docker run -it filiosoft/rsync bash
```

### Use as base image
```Dockerfile
FROM filiosoft/rsync:latest
```