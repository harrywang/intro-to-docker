# About
code for the official docker tutorials
- bulletin-board-app: [Get started with Docker](https://docs.docker.com/get-started/)
- compose-test: [Get started with Docker Compose](https://docs.docker.com/compose/gettingstarted/)

docker commands:

```
$ docker --version
$ docker image ls
$ docker container ls --all
$ docker image build . -t bulletinboard:1.0
$ docker container run --publish 8000:8080 --detach --name bb bulletinboard:1.0
$ docker container rm --force bb
$ docker image tag bulletinboard:1.0 harrywang/bulletinboard:1.0
$ docker image push harrywang/bulletinboard:1.0
$ docker image prune  # remove used image
$ docker system prune --all # Remove all unused images not just dangling ones
$ docker system prune --volumes # Prune volumes
```

In compose-test folder, try docker compose commands and go to http://0.0.0.0:5000/

```
$ docker-compose -v
$ docker-compose build
$ docker-compose up
$ docker-compose stop
$ docker-compose up -d
$ docker-compose up -d --build
$ docker-compose run web env # run command for services
$ docker-compose down
$ docker-compose down --volumes
```
