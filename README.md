# Verdaccio + Docker Compose [npm-local-server]

Create a persistence NPM Local Server with Verdaccio and Docker

Instructions:

Create all needed folders

```console
mkdir verdaccio && cd verdaccio
mkdir conf
mkdir storage
mkdir logs
mkdir plugins
```

Create verdaccio configuration file: config.yaml 

```console
touch conf/config.yaml
```

Create docker-compose.yaml

```console
touch docker-compose.yaml
```

Run the service

```console
docker-compose up -d
```

Or you can run directly without docker-compose

```console
docker run -it --detach \
    --publish 4873:4873 \
    --volume `pwd`/conf:/verdaccio/conf \
    --volume `pwd`/storage:/verdaccio/storage \
    --volume `pwd`/plugins:/verdaccio/plugins \
    --name verdaccio \
    verdaccio/verdaccio
```
=======
