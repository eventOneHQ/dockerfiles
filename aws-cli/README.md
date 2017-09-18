# AWS-CLI in Docker
[![](https://images.microbadger.com/badges/image/filiosoft/aws-cli.svg)](http://microbadger.com/images/filiosoft/aws-cli "Get your own image badge on microbadger.com")
[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/aws-cli.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/aws-cli)

[AWS-CLI](https://aws.amazon.com/cli/) Docker image. 
## WARNING: This `Dockerfile` has been moved to the Filiosoft GitLab. You can find it [here](https://developers.filiosoft.com/docker/aws-cli). 
### based on [alpine:3.3](https://hub.docker.com/_/alpine/)
----
### Pull from Docker Hub
```
docker pull filiosoft/aws-cli:latest
```

### Build from GitHub
```
docker build -t filiosoft/aws-cli github.com/filiosoft/dockerfiles:aws-cli
```

### Run image
```
docker run -it filiosoft/aws-cli bash
```

### Use as base image
```Dockerfile
FROM filiosoft/aws-cli:latest
```