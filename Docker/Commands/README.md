# 🔴 Docker Commands

## docker run

```bash
docker run [OPTIONS] IMAGE[:TAG|@DIGEST] [COMMAND] [ARG...]
```

## docker ps

```bash
docker ps [OPTIONS]
```

## docker images

```bash
docker images [OPTIONS] [REPOSITORY[:TAG]]
```

## docker pull

```bash
docker pull [OPTIONS] NAME[:TAG|@DIGEST]
```

## docker push

```bash
docker push [OPTIONS] NAME[:TAG]
```

## docker rm

```bash
docker rm [OPTIONS] CONTAINER [CONTAINER...]
```

## docker rmi

```bash
docker rmi [OPTIONS] IMAGE [IMAGE...]
```

## docker exec

```bash
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
```

## docker logs

```bash
docker logs [OPTIONS] CONTAINER
```

## docker commit

```bash
docker commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]
```

## docker tag

```bash
docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]
```

## docker build

```bash
docker build [OPTIONS] PATH | URL | -
```

## docker login

```bash
docker login [OPTIONS] [SERVER]
```

## docker logout

```bash
docker logout [SERVER]
```

## docker search

```bash
docker search [OPTIONS] TERM
```

## docker info

```bash
docker info [OPTIONS]
```

## docker version

```bash
docker version [OPTIONS]
```

## docker top

```bash
docker top [OPTIONS] CONTAINER [ps OPTIONS]
```

## docker attach

```bash
docker attach [OPTIONS] CONTAINER
```

## docker cp

```bash
docker cp [OPTIONS] CONTAINER:SRC_PATH DEST_PATH|- OR SRC_PATH|- CONTAINER:DEST_PATH
```

## docker diff

```bash
docker diff [OPTIONS] CONTAINER
```

## docker events

```bash
docker events [OPTIONS]
```

## docker export

```bash
docker export [OPTIONS] CONTAINER
```

## docker history

```bash
docker history [OPTIONS] IMAGE
```

## docker import

```bash
docker import [OPTIONS] file|URL|- [REPOSITORY[:TAG]]
```

## docker kill

```bash
docker kill [OPTIONS] CONTAINER [CONTAINER...]
```

## docker load

```bash
docker load [OPTIONS]
```

## docker pause

```bash
docker pause [OPTIONS] CONTAINER [CONTAINER...]
```

## docker port

```bash
docker port [OPTIONS] CONTAINER [PRIVATE_PORT[/PROTO]]
```

## docker rename

```bash
docker rename [OPTIONS] CONTAINER NEW_NAME
```

## docker restart

```bash
docker restart [OPTIONS] CONTAINER [CONTAINER...]
```

## docker save

```bash
docker save [OPTIONS] IMAGE [IMAGE...]
```

## docker start

```bash
docker start [OPTIONS] CONTAINER [CONTAINER...]
```

## docker stats

```bash
docker stats [OPTIONS] [CONTAINER...]
```

## docker stop

```bash
docker stop [OPTIONS] CONTAINER [CONTAINER...]
```

## docker system

```bash
docker system [OPTIONS] COMMAND
```

## docker unpause

```bash
docker unpause [OPTIONS] CONTAINER [CONTAINER...]
```

## docker update

```bash
docker update [OPTIONS] CONTAINER [CONTAINER...]
```

## docker wait

```bash
docker wait [OPTIONS] CONTAINER [CONTAINER...]
```

# ℹ️ Dockerfile

## `FROM`
The FROM instruction initializes a new build stage and sets the Base Image for subsequent instructions.

```bash
FROM <image>[:<tag>]
```

## `RUN`
The RUN instruction will execute any commands in a new layer on top of the current image and commit the results. The resulting committed image will be used for the next step in the Dockerfile.

```bash
RUN <command>
```

### `CMD`
The main purpose of a CMD is to provide defaults for an executing container.

```bash
CMD ["executable","param1","param2"]
```

### `EXPOSE`
Informs Docker that the container listens on the specified network ports at runtime.

```bash
EXPOSE <port> [<port>/<protocol>...]
```

### `ENV`
The ENV instruction sets the environment variable <key> to the value <value>. This value will be in the environment for all subsequent instructions in the Dockerfile as well as for the image when it is run in a container.

```bash
ENV <key> <value>
```

### `ADD`
The ADD instruction copies new files, directories or remote file URLs from <src> and adds them to the filesystem of the image at the path <dest>.

```bash
ADD <src>... <dest>
```

### `COPY`
The COPY instruction copies new files or directories from <src> and adds them to the filesystem of the container at the path <dest>.

```bash
COPY <src>... <dest>
```

### `ENTRYPOINT`
An ENTRYPOINT allows you to configure a container that will run as an executable.

```bash
ENTRYPOINT ["executable", "param1", "param2"]
```

### `VOLUME`
The VOLUME instruction creates a mount point with the specified name and marks it as holding externally mounted volumes from native host or other containers.

```bash
VOLUME ["/data"]
```
