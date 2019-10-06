# rmq-es-logstash

Logstash docker container that using RabbitMQ as input and Elasticsearch as output

## Getting Started

These instructions will cover usage information and for the docker container

### Prerequisities

In order to run this container you'll need docker installed.

- [Windows](https://docs.docker.com/windows/started)
- [OS X](https://docs.docker.com/mac/started/)
- [Linux](https://docs.docker.com/linux/started/)

### Steps

#### Build container

```shell
docker build . -t=rmq-es-logstash
```

#### Run container

```shell
docker run --rm -it --env ELASTICSEARCH_URL --env RABBIT_HOST --env RABBIT_USERNAME --env RABBIT_PASSWORD --env RABBIT_PORT --env RABBIT_VHOST --env RABBIT_EXCHANGE_NAME --env RABBIT_EXCHANGE_TYPE --env RABBIT_QUEUE_NAME --env RABBIT_RETRY_INTERVAL --env RABBIT_DURABLE rmq-es-logstash:latest
```
