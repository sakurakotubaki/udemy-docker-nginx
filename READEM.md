# Nginx Container

1. image pull from Docker Hub

The correct syntax for running a container with port mapping is:
```shell
docker run -p 8080:80 nginx
```

2. port maping
`-p(--publish)

**Or with more options:**

```shell
docker run --name container-name -p 8080:80 -d nginx
```

URL:

http://localhost:8080/

Option to delete the container when it is stopped

1. run
```shell
docker run --rm -p 8080:80 nginx
```

2. docker stop
```shell
# ps command
docker ps
# stop
docker stop 5662dcb5f00f
```

* Name the container

```shell
# Delete when stopped
docker run --rm -p 8080:80 --name my-nginx nginx:1.27.4
```

* case stop
```shell
# stop
docker stop my-nginx
# rm
docker rm my-nginx
```

* Background

```shell
# run background
docker run -d -p 8080:80 --name my-nginx nginx:1.27.4
# stop
docker stop my-nginx
```