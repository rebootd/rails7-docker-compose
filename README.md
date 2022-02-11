# README

This README would normally document whatever steps are necessary to get the
application up and running.


## source article
https://docs.docker.com/samples/rails/
- this plus updating some versions

## pull to start a new app
```
> git init foo
> cd foo
> git pull https://github.com/rebootd/rails7-docker-compose.git
```


## steps
```
> touch Gemfile.lock
> docker-compose run --no-deps web rails new . --force --database=postgresql
> sudo chown -R $USER:$USER .
> docker-compose build
> docker-compose up
> docker-compose run web rake db:create
> docker-compose up
# attach to the running container, example container name: rails7-docker-compose_web_1
> docker exec -i -t rails7-docker-compose_web_1 /bin/bash
```
