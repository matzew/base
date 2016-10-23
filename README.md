# Base Docker image for JBoss community projects

This repository contains base image that is used to build the portfolio of Docker images for JBoss community projects. 

## Base image

This image is used as a base image for *all* JBoss community images. It provides a base layer that includes:

1. A `jboss` user (uid/gid `1000`) with home directory set to `/opt/jboss`
2. A few tools that may be useful when extending the image or installing software, like `unzip`.

### Operating system

This image uses CentOS 7 on aarch64/arm64.

### Working directory

This image has the working directory set to `/opt/jboss`, which is the `jboss` user home directory at the same time.

### Availability

The `Dockerfile` is available in the `aarch64` branch and the docker image can be found at Docker HUB as `project31/aarch64-jboss-base:latest` (https://hub.docker.com/r/project31/aarch64-jboss-base/) - built on Pine64.
