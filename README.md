# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## article
https://docs.docker.com/samples/rails/
- this plus updating some versions

## steps
```
> docker-compose run --no-deps web rails new . --force --database=postgresql
> sudo chown -R $USER:$USER .
> docker-compose build
> docker-compose up
> docker-compose run web rake db:create
> docker-compose up
# attach to the running container, example container name: rails7-docker-compose_web_1
> docker exec -i -t rails7-docker-compose_web_1 /bin/bash
```
