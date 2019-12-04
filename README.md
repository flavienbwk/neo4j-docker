# Neo4j Docker

Dockerized Neo4j instance with compose.

## Run !

```
docker-compose up -d
```

And visit : [`localhost:7474`](localhost:7474)

## Architecture

|Directory|Intent|
|----|----|
|`conf/`| Contains the `neo4j.conf` config file |
|`data/`| Used to persist the Neo4j data |
|`import/`| Place your files there to import data (e.g: with `LOAD CSV`) |
|`logs/`| Logs of your Neo4j instance will appear here |

## Importing files

To import files, place your files inside the `import/` directory and you will be able to import them through Cypher commands.