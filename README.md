# docker-cheatsheet

- `docker ps`: Show all running containers
- `docker ps -a`: Show all running/stopped containers, that existed on sometime in docker

* `docker images`: Show all the docker present on the system.
* `docker remove <container_name> | <container_id>`: Delete docker container

* `docker image rm <image_id> | <image_name>`: Delete docker images from your local machine.

- `docker stop <container_hash> or <container_name>`: Stop a running container
- `docker start <container_hash>`: Run a stopped container
- `docker run -d -p <host_machine_port>:<container_port> <image_name>:<image_tag>`: Run a container from image in detached mode and expose its port.

* `docker logs <container_name>`: Show the logs of the container, typically used for detached containers.

* `docker export <container_name> > contents.tar`: It outputs the contents of your container in a .tar file.

* `docker build -t portfolio-app:1.0 .`: Build docker image of this name and version, from this location, the location in which the Dockerfile is located

* `docker kill <container_id>`: Kill runninf docker container

### Reposity v/s Registry

## Registry

- A service providing storage for you docker images, that can be hosted anywhere like AWS ECR etc.
- A registry can have multiple images or we can say multiple repositories for you application.

# Repository

- Collection of related images with same name, but with different versions.
