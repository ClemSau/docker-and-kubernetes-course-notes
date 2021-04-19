# Docker Compose with multiple local containers

In most cases, we won't create containers with all sub-app composing our main app. It would present issues of scalability and consistency of our app.
For instance, if we were to start multiple containers containing a redis instance, they would all have different informations.

## Docker compose

`docker-compose.yaml` is an additional file that is used to run mutliple containers at once. In addition to some uptakes, like shared private network.
