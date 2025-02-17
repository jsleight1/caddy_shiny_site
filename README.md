

This repo contains a simple docker compose file which allows
deployment of multiple shiny applications using Caddy as a proxy server.

This is based on a series of tutorials found at:
 - https://hosting.analythium.io/host-shiny-apps-with-docker/#install-caddy-server
 - https://hosting.analythium.io/shiny-apps-with-docker-compose-part-1-development/

Shiny apps used are:
 - [example docker shiny](https://github.com/jsleight1/example_docker_shiny/tree/main)
 - [lgbf](https://github.com/jsleight1/LGBF/tree/main)
 - [example_database_shiny](https://github.com/jsleight1/example_database_shiny)

The docker compose file is launched using

```
docker compose up -d
```

where .env is a local file:

```
dbpath=PATH_TO_DATABASE
```

`dbpath` is a path to the directory storing the ozone.duckdb database file 
for [example_database_shiny](https://github.com/jsleight1/example_database_shiny) on
your local machine.

Shiny applications can then navigated to from:

```
localhost:8000
```
