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
