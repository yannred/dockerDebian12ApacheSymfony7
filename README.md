# dockerDebian12ApacheSymfony7
Generate a docker image based on Php 8.3.2 and Debian Bookworm for Symfony 7

## Build for locally usage
> docker build -t debian12-apache-symfony7 .

## Run
> docker-compose up -d

## Publish on Docker hub
```bash
docker login -u "ityannred" docker.io
docker build -t ityannred/apache-symfony7 .
docker tag debian12-apache-symfony7:latest ityrannred/debian12-apache-symfony7:latest
docker push ityrannred/debian12-apache-symfony7:latest
```