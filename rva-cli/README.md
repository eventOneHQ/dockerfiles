# RVA CLI
Node.js 6 with rsync, aws-cli, and rva-cli.

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/rva-cli.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/rva-cli/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/rva-cli:latest.svg)](https://imagelayers.io/?images=filiosoft/rva-cli:latest)

## WARNING: This `Dockerfile` has been moved to the Filiosoft GitLab. You can find it [here](https://gitlab.filiosoft.com/docker/rva-cli). 

### based on [node:6](https://hub.docker.com/r/_/node/)
----
### Pull from Docker Hub
```
docker pull filiosoft/rva-cli:latest
```

### Build from GitHub
```
docker build -t filiosoft/rva-cli https://raw.githubusercontent.com/Filiosoft/dockerfiles/master/rva-cli/Dockerfile
```

### Run image
```
docker run -it filiosoft/rva-cli bash
```

### Use as base image
```Dockerfile
FROM filiosoft/rva-cli:latest
```