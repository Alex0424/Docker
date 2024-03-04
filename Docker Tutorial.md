# Docker

Download Docker

https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe

Install wsl in terminal

https://learn.microsoft.com/en-us/windows/wsl/install

# Usefull Docker Commands

`docker` + `stop`/`remove` + `container_name`

container list: `docker ps`

`docker images`

`docker stats`

`docker run -t -d -p host_port:docker_container_port --name new_container_name image_name`

# Start
```
docker pull centos:latest
docker run -d -t --name container_name centos
```
