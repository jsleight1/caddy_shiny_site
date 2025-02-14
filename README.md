

This repo contains a simple docker compose file which allows
deployment of multiple shiny applications using Caddy as a proxy server.

This is based on a series of tutorials found at:
 - https://hosting.analythium.io/host-shiny-apps-with-docker/#install-caddy-server
 - https://hosting.analythium.io/shiny-apps-with-docker-compose-part-1-development/

Shiny apps used are:
 - [example docker shiny](https://github.com/jsleight1/example_docker_shiny/tree/main)

The docker compose file is launched using

```
docker compose up -d
```

Shiny applications can then navigated to from:

```
localhost:8000
```