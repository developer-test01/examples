## Building the Docker images

```console
$ docker build -t gcr.io/nttd-platformtec/gb-frontend:v5 php-redis

$ docker build -t gcr.io/nttd-platformtec/gb-redisslave:v2 redis-slave
```

Building Multi-architecture docker images

```console
$ make -C php-redis

$ make -C redis-slave
```

Push:

```console
$ make -C php-redis all-push

$ make -C redis-slave all-push
```
