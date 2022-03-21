# Dockerfile vs Docker compose

A Dockerfile is a text document that contains all the commands/Instruction a 
user could call on the command line to assemble an image. 

For example:

```docker
FROM centos:latest
LABEL maintainer="collabnix"
RUN yum update -y && \
	yum install -y httpd net-tools && \
	mkdir -p /run/httpd 
EXPOSE 80
ENTRYPOINT apachectl "-DFOREGROUND"
```

Using docker build commmand we can build an image from a Dockerfile.

Docker Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration. By default, docker-compose expects the name of the Compose file as docker-compose.yml or docker-compose.yaml. If the compose file have different name we can specify it with -f flag.

A docker-compose.yml looks like this:


```docker
version: '3'
services:
  web:
    build: .
    ports:
    - "5000:5000"
    volumes:
    - .:/code
    - logvolume01:/var/log
    links:
    - redis
  redis:
    image: redis
volumes:
  logvolume01: {}
```
