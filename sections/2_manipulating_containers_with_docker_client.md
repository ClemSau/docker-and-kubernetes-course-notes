# Manipulating containers with docker client

## How does docker runs on a computer

Docker is a linux VM, so it present some linux specific features like:
- Namespacing: Isolating resources per process (or group of precesses)
- Control groups (cgroups): Limit the amount of resources used per process

Creating and running a container from an image: `docker run {image_name}`

![Docker run](img/2_1.png)

eg: `docker run busybox echo bye world`

## Listing running containers

`docker ps`

![Docker ps](img/2_2.png)