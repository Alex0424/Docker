# Docker commands

| Info                                 | Command (Linux)                                                | 
| ------------------------------------ | -------------------------------------------------------------- |
| test a container (its quick)         | docker run hello-world                                         |
| start a new conainer                 | docker run --name imagename -d -p 9080:80 nginx                |
| build docker image from a Dockerfile | docker build -t imagename DockerfilePath                       |
| list images                          | docker images                                                  |
| list running containers              | docker ps                                                      |
| list all containers                  | docker ps -a                                                   |
| inspect container                    | docker inspect conainer_name                                   |
| remove image                         | docker rmi image                                               |




# Push image to hub

```
docker pull image_from_docker_hub
docker run hello-world
vim Dockerfile
docker build -t <your_username>/my-private-repo .
docker run <your_username>/my-private-repo
docker push <your_username>/my-private-repo
```
