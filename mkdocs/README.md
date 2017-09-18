# MkDocs in Docker
[![](https://images.microbadger.com/badges/image/filiosoft/mkdocs.svg)](http://microbadger.com/images/filiosoft/mkdocs "Get your own image badge on microbadger.com")
[![Docker Pulls](https://img.shields.io/docker/pulls/filiosoft/mkdocs.svg?style=flat-square)](https://fsft.us/d-mkdocs)

[MkDocs](http://www.mkdocs.org/) Docker image. 

## WARNING: This `Dockerfile` has been moved to the Filiosoft GitLab. You can find it [here](https://developers.filiosoft.com/docker/mkdocs). 

### based on [python:alpine](https://hub.docker.com/_/python/)
----
### Pull from Docker Hub
```
docker pull filiosoft/mkdocs:latest
```

### Build from GitHub
```
docker build -t filiosoft/mkdocs github.com/filiosoft/dockerfiles:mkdocs
```

### Run image
```
docker run -it filiosoft/mkdocs bash
```

### Use as base image
```Dockerfile
FROM filiosoft/mkdocs:latest
```