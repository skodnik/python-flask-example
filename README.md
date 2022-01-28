# Пример простого Flask web приложения

## Prerequisites
Make sure you have already installed both [Docker Engine](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/). You don’t need to install Python or Redis, as both are provided by Docker images.

## Clone
```bash
git clone git@github.com:skodnik/python-flask-example.git composetest
```

## Init
```bash
cd composetest
docker-compose up
```

## Run
```bash
http://127.0.0.1:5000/
```

Источник - [docs.docker.com/compose/gettingstarted](https://docs.docker.com/compose/gettingstarted/)