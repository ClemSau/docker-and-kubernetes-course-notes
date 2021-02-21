# Dive into docker 

## Why use docker
Docker makes it easy to install and run softwares on any giver device.
eg: If I wanted to run redis on my computer, I'd need to go through multiple steps and probably install third party programs, all that tailored to my OS. With docker, the process is uniformized and simplified. It can even be scripted.

Docker is a whole ecosystem:
- Docker client
- Docker server
- Docker Machine
- Docker Images
- Docker Hub
- Docker Compose

### What is an image

Single file with all the deps and configs required to run a program.

### What is a container

An instance of an image. Runs a program.

### Docker for Windows/Mac

- Docker client (CLI)
- Docker server (Docker Daemon)

## Using the docker client

When we run `docker run hello-world`, here what happens:
- The command is processed by the docker client (CLI)
- It is passed to the docker server
- The docker server check in our image cache (the local images) for the ran image
- If the image is not in the image cache, it reach to the docker hub, and check if the image exist. If so, it downloads the image into the image cache, and runs it.

