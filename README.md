# Nginx Alpine Linux - Docker image

[![Latest Version](https://img.shields.io/github/v/release/kiwfy/nginx-alpine.svg?style=flat-square)](https://github.com/kiwfy/nginx-alpine/releases)
[![Build Status](https://img.shields.io/github/workflow/status/kiwfy/nginx-alpine/CI?label=ci%20build&style=flat-square)](https://github.com/kiwfy/nginx-alpine/actions?query=workflow%3ACI)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

Docker image with Nginx using Alpine Linux OS

### How to use this image

Requires [Docker](https://www.docker.com/get-started).

Before get the image is necessary [authenticate](https://docs.github.com/pt/packages/using-github-packages-with-your-projects-ecosystem/configuring-docker-for-use-with-github-packages) in Github Package

You can run the container and service like so:

```sh
docker run -d -p 80:80 docker.pkg.github.com/kiwfy/nginx-alpine/nginx-alpine:latest
```

### Docker with compose tool

It's a good way to use [docker-compose](https://docs.docker.com/compose/). Example:

```
version: '3.7'
services:
    nginx:
        image: docker.pkg.github.com/kiwfy/nginx-alpine/nginx-alpine:latest
        container_name: nginx
        ports:
            - 80:80
        volumes:
            - ./:/var/www/html
```

### Development

Want to contribute? Great!

Make a change in image and be careful with your updates!

**Kiwfy - Open your code, open your mind!**
