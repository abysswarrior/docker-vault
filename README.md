# Docker Vault
A place to keep my docker-compose collections.

## Pre-requirements

* most of these docker containers use `app-network` network
use this command to create it:

```bash
docker network create app-network 
```

---
## List of Docker-Compose Files

* [PostgreSQL + PgAdmin](#postgresql-and-pgadmin)
* [Redis + Redisinsight](#redis-and-redisinsight)
* [RabbitMQ](#rabbitmq)

---
#### PostgreSQL and PgAdmin

_A collection of Database tools that i need for almost every django project_

* **use a volume to persist data**
* **use a `app-network` network to see other containers in DNS scoop**
* [**See yml file**](./PostgreSQL_and_pgAdmin/docker-compose.yml)

---
#### Redis and Redisinsight

_A set of useful redis DB and redisinsight web UI tools to work with redis_

* **use a volume to persist data**
* **use a `app-network` network to see other containers in DNS scoop**
* [**See yml file**](./Redis_and_Redisinsight/docker-compose.yml)

---
#### RabbitMQ

_Mostly used celery broker_

* **needs a `data` directory to persist data**
* [**See yml file**](./RabbitMQ/docker-compose.yml)

