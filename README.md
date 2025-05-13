# dockerDebian12ApacheSymfony7
Generate a docker image based on Php 8.3.2 and Debian Bookworm for Symfony 7

## Build for locally usage
> docker build -t debian12-apache-symfony7 .

## Run
> docker-compose up -d

## Publish on Docker hub

Pour x86_64
```bash
docker login -u "ityannred" docker.io && \
docker build -t ityannred/debian12-apache-symfony7 . && \
docker tag debian12-apache-symfony7:latest ityannred/debian12-apache-symfony7:latest && \
docker push ityannred/debian12-apache-symfony7:latest
```

Pour ARM64
```bash
docker login -u "ityannred" docker.io && \
docker build --platform linux/arm64/v8 -t debian12-apache-symfony7:arm64 .
docker tag debian12-apache-symfony7:arm64 ityannred/debian12-apache-symfony7:arm64 && \
docker push ityrannred/debian12-apache-symfony7:arm64
```
