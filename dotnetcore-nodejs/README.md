# dotnetcore-nodejs
Microsoft's .NET Core image with Node.js 6 and Bower added! 

## WARNING: This `Dockerfile` has been moved to the Filiosoft GitLab. You can find it [here](https://gitlab.filiosoft.com/docker/dotnetcore-node). 

[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/dotnetcore-nodejs.svg?style=flat-square)](https://hub.docker.com/r/filiosoft/dotnetcore-nodejs/)
[![ImageLayer](https://badge.imagelayers.io/filiosoft/dotnetcore-nodejs:latest.svg)](https://imagelayers.io/?images=filiosoft/dotnetcore-nodejs:latest)

### Pull from Docker Hub
```
docker pull filiosoft/dotnetcore-nodejs:latest
```

### Build from GitHub
```
docker build -t filiosoft/dotnetcore-nodejs github.com/filiosoft/dockerfiles:dotnetcore-nodejs
```

### Run image
```
docker run -it filiosoft/dotnetcore-nodejs bash
```

### Use as base image
```Dockerfile
FROM filiosoft/dotnetcore-nodejs:latest
```