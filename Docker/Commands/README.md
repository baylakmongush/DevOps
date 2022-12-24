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
