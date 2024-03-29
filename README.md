# Neo4j Docker

Dockerized Neo4j instance with compose.

## Run

```bash
docker-compose up -d
```

> To edit configuration, [see the official documentation](https://neo4j.com/docs/operations-manual/current/docker/configuration/).

You can now visit [`localhost:7474`](localhost:7474) (default credentials: `neo4j`/`neo4jj`)

## Architecture

| Directory | Intent                                                       |
| --------- | ------------------------------------------------------------ |
| `data/`   | Used to persist the Neo4j data                               |
| `import/` | Place your files there to import data (e.g: with `LOAD CSV`) |
| `logs/`   | Logs of your Neo4j instance will appear here                 |

## Importing files

To import files, place your files inside the `import/` directory and you will be able to import them through Cypher commands.
