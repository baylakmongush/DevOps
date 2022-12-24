# Docker

## Architecture
<img src="Images/Arch.png" height="200" align="center">

## Dockerfile
* Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image.
* Dockerfile is a set of instructions that Docker will execute in order to build an image.

## Dockerfile commands
* FROM
* RUN
* CMD
* EXPOSE
* ENV
* ADD
* COPY
* ENTRYPOINT
* VOLUME
* USER
* WORKDIR
* ARG
* ONBUILD
* STOPSIGNAL
* HEALTHCHECK
* SHELL
* LABEL
* MAINTAINER
* ARG

## Dockerfile example
```Dockerfile
FROM ubuntu:latest
RUN apt-get update && apt-get install -y python3-pip python3-dev
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt
ENTRYPOINT [ "python3" ]
CMD [ "app.py" ]
```

