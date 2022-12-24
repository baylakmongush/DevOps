# 🔴 Docker Installation

## Linux

### Ubuntu

```bash
sudo apt-get update
sudo apt-get install docker.io
```

### CentOS

```bash
sudo yum install docker
```

### Fedora

```bash
sudo dnf install docker
```

### Arch Linux

```bash
sudo pacman -S docker
```

### Debian

```bash
sudo apt-get update
sudo apt-get install docker.io
```

### Alpine

```bash
sudo apk add docker
```

### RHEL

```bash
sudo yum install docker
```

## Windows

### Windows 10

1. Download and install Docker Desktop for Windows from the Docker Hub.
2. Open Docker Desktop and go to Settings > Resources > File Sharing.
3. Add the drive where your code is located.
4. Click Apply & Restart.
5. Open a terminal and run docker run hello-world to verify that Docker is installed correctly.
6. To run the Docker CLI without sudo, create a Unix group called docker and add users to it. When the Docker daemon starts, it makes the ownership of the Unix socket read/writable by the docker group.
7. To create the docker group and add your user:
```bash
# Create the docker group.
sudo groupadd docker

# Add your user to the docker group.
sudo usermod -aG docker $USER

# Log out and log back in so that your group membership is re-evaluated.

# Verify that you can run docker commands without sudo.
docker run hello-world
```

### Windows 7

1. Download and install Docker Toolbox for Windows from the Docker Hub.
2. Open a terminal and run docker run hello-world to verify that Docker is installed correctly.
3. To run the Docker CLI without sudo, create a Unix group called docker and add users to it. When the Docker daemon starts, it makes the ownership of the Unix socket read/writable by the docker group.
4. To create the docker group and add your user:
```bash
# Create the docker group.
sudo groupadd docker

# Add your user to the docker group.
sudo usermod -aG docker $USER

# Log out and log back in so that your group membership is re-evaluated.

# Verify that you can run docker commands without sudo.
docker run hello-world
```

## Mac

### Mac OS X

1. Download and install Docker Desktop for Mac from the Docker Hub.
2. Open Docker Desktop and go to Settings > Resources > File Sharing.
3. Add the drive where your code is located.
4. Click Apply & Restart.
5. Open a terminal and run docker run hello-world to verify that Docker is installed correctly.
6. To run the Docker CLI without sudo, create a Unix group called docker and add users to it. When the Docker daemon starts, it makes the ownership of the Unix socket read/writable by the docker group.
7. To create the docker group and add your user:
```bash
# Create the docker group.
sudo groupadd docker

# Add your user to the docker group.
sudo usermod -aG docker $USER

# Log out and log back in so that your group membership is re-evaluated.

# Verify that you can run docker commands without sudo.
docker run hello-world
```