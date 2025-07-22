# Summary

Dockerized postgre with ja locale.
official postgre image: https://hub.docker.com/_/postgres/

## PostgreSQL Configuration

This image is configured with the following settings for logical replication:
- `wal_level=logical`: Enables logical replication
- `max_replication_slots=10`: Maximum number of replication slots
- `max_wal_senders=10`: Maximum number of concurrent WAL sender processes

# Local Build

```sh
$ docker build -t kahnabell/postgre-ja:latest .
```
