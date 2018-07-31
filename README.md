# python3-awscli-docker

## How to build this image locally

Run the following command

```
$ docker build -t python3-awscli-docker .
```

To tag for dockerhub

```
$ docker tag python3-awscli-docker vcard/python3-awscli-docker
```

To push to docker hub

```
$ export DOCKER_ID_USER="username"
$ docker login
$ docker push vcard/python3-awscli-docker
```

## How to use this image

Run the following commands:

```
$ docker pull vcard/python3-awscli-docker
```

Run the docker container in the background with the following command

```
$ docker run  -d -t --name python3-awscli-docker vcard/python3-awscli-docker
```

Ensure aws-cli, docker-ce and dotnetcore is installed

```
$ docker exec -it python3-awscli-docker  ../bin/sh
```

Run the following commands:

```
$ dotnet --version
$ aws --version
$ docker --version
$ exit
```
