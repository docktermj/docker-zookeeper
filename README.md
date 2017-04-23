# docker-zookeeper

## Build

```console
sudo docker build \
    --tag dockter/zookeeper:0.1 \
    .
```

References:

- [docker build](https://docs.docker.com/edge/engine/reference/commandline/build/)

## Run

```console
sudo docker run \
    --interactive \
    --tty \
    --publish 2181:2181 \
    --name zookeeper \
    dockter/zookeeper:0.1
```

References:

- [docker run](https://docs.docker.com/edge/engine/reference/commandline/run/)


## Remove

```console
sudo docker rm zookeeper
```

## Push to DockerHub

[dockter/zookeeper](https://hub.docker.com/r/dockter/zookeeper/)

```console
sudo docker login
sudo docker push dockter/zookeeper:0.1
```

References:

- [docker login](https://docs.docker.com/edge/engine/reference/commandline/login/)
- [docker push](https://docs.docker.com/edge/engine/reference/commandline/push/)

## Technical details

FROM [openjdk:8-jre-alpine](https://github.com/docker-library/openjdk/blob/master/8-jre/Dockerfile)

## References

1. [Apache ZooKeeper](https://zookeeper.apache.org/)