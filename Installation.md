# Docker

Download Docker

https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe

Install wsl in terminal

https://learn.microsoft.com/en-us/windows/wsl/install

# Start

open your linux terminal

```
mkdir docker && cd docker && vim Dockerfile
```
add commands in text file:
```
FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y vim
```
```
docker build .
docker images #copy your new image id
docker run /home/your_user/docker:/mnt -it --name demo your_new_image_id
```
# Random Docker Commands

`docker` + `stop`/`remove` + `container_name`

container list: `docker ps`

`docker images`

`docker stats`

`docker run -t -d -p host_port:docker_container_port --name new_container_name image_name`

transfer everything from docker dir to mnt dir in new container: `docker run -v /home/alex/docker:/mnt -it 3db8720ecbf5`

```
docker pull centos:latest
docker run -d -t --name container_name centos
```
