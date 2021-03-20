# Building custom images through docker server

## Flow of creating Docker Images

The image configuration occures in the `.Dockerfile`

To create one we will follow a specific flow:
- Specify a base image
- Run some commands to install additional programs
- Specify a command to run on container startup

## Building a Docker image

Example of a `.Dockerfile` which runs redis:

```
# Use an existing docker image as a base
FROM alpine

# Dowload and install a dependency
RUN apk add --update redis

# Tell the image what to do when it starts as a container
CMD ["redis-server"]
```

Then we build the image with the command `docker build .`

Which return an id you can the run with `docker run {image_id}`