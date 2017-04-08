# Using docker to avoid installing MySQL

You can use docker to isolate binary dependencies without ruining your developer experience.

Docker offers tool called `docker-compose` it is a tool for defining and running multi-container Docker applications. In our case it's the app and database containers.

To use it we first need to define two files. `Dockerfile` configures how to setup our application and `docker-compose.yml` configures the infrastructure.

[Read more](https://github.com/docker/compose)

## Useful commands

Run the app
```bash
docker-compose up
```

List all containers and their state
```bash
docker-compose ps
```

Run the app in background
```bash
docker-compose up -d
```

You can then stop the app using
```bash
docker-compose stop
```
