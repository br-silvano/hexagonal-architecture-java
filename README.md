# Hexagonal architecture (software)

## Install all dependencies and run the application
```bash
$ docker-compose -f docker-compose.dev.yml up --build
```

## Run application
```bash
$ docker-compose -f docker-compose.dev.yml up
```

## Remove all containers
```bash
$ docker rm $(docker ps -aq) -f
```

## Remove all volumes
```bash
$ docker volume rm $(docker volume ls --format {{.Name}}) -f
```

## Remove all images
```bash
$ docker image rm $(docker images --format {{.ID}}) -f
```
