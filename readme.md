# Templates for docker-compose

### How to start a container with docker-compose

```bash
docker-compose up -d
```

### How to stop a container with docker-compose

```bash
docker-compose down
```

### How to start a container with docker-compose and build it

```bash
docker-compose up -d --build
```

### How to start a container with docker-compose and rebuild it

```bash
docker-compose up -d --build --force-recreate
```

### Traefik folder

The traefik folder contains the configuration for the reverse proxy.
the files is ready to use with docker-compose, but you need to change the domain name in the file `traefik.toml` and the file `docker-compose.yml`.

I use grafana and prometheus for monitoring, but you can remove it if you don't need it.

I use portainer for managing the docker containers, but you can remove it if you don't need it.

Enjoy!
