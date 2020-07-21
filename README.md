# Verdaccio + Docker Compose

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
touch docker-compose.yml
```

Run the service

```console
docker-compose up -d
```
