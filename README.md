# Golang 1.10beta1 Docker image on alpine 3.6

[![DockerPulls](https://img.shields.io/docker/pulls/banzaicloud/golang.svg)](https://registry.hub.docker.com/u/banzaicloud/golang/)
[![DockerStars](https://img.shields.io/docker/stars/banzaicloud/golang.svg)](https://registry.hub.docker.com/u/banzaicloud/golang/)

The official [golang docker repo](https://hub.docker.com/r/_/golang/) doesn't contains the beta release of 1.10 yet.
This repo is the fork of [docker-library/golang](https://github.com/docker-library/golang/tree/master/1.9/alpine3.6),
but only cares about golang on alpine3.6 (smallest, and most secure)

## Usage

Use it as ususal. If you were using **golang/alpine** or **golang/1.9.2-alpine3.6** or similar,
just replace the image name to **banzaicloud/golang:v1.10beta1**
```
$ docker run banzaicloud/golang:v1.10beta1 go version
go version go1.10beta1 linux/amd64
```

## Changes from original

2 [changes](https://github.com/banzaicloud/docker-golang/commit/d1b5e6b7a90b2cba6e30659024d942616279fe39) were made:
- source patches are removed (they dont fit the 1.10 branch, so they are just removed them careless)
- GOLANG_VERSION env variable is set to 1.10beta1 



