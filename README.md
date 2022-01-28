# Пример простого Flask web приложения

## Prerequisites
Make sure you have already installed both [Docker Engine](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/). You don’t need to install Python or Redis, as both are provided by Docker images.

## Clone
```bash
git clone git@github.com:skodnik/python-flask-example.git composetest
```

## Init + Run
```bash
cd composetest
docker-compose up
```
Enter http://localhost:5000/ or http://127.0.0.1:5000/ in a browser to see the application running.

## Detached docker processes
If you want to run your services in the background, you can pass the -d flag (for “detached” mode) to docker-compose up and use docker-compose ps to see what is currently running:
```bash
docker-compose up -d
```

## Stop 
```bash
docker-compose stop
```

## Cleanup
You can bring everything down, removing the containers entirely, with the down command. Pass --volumes to also remove the data volume used by the Redis container:
```bash
docker-compose down --volumes
```

Источник - [docs.docker.com/compose/gettingstarted](https://docs.docker.com/compose/gettingstarted/)