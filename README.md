# docker-zookeeper

FROM [openjdk:8-jre-alpine](https://github.com/docker-library/openjdk/blob/master/8-jre/Dockerfile)

## Build

```console
sudo docker build -t dockter/zookeeper:0.1 .
```

## Run

```console
sudo docker run -p 2181:2181 -i -t dockter/zookeeper:0.1
```

## Push to Docker Hub

[dockter/zookeeper](https://hub.docker.com/r/dockter/zookeeper/)

```console
sudo docker login
sudo docker push dockter/zookeeper:0.1
```