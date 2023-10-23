# compose-mysql

Docker Compose using Docker Hub [Postgres](https://hub.docker.com/_/postgres)


### Running Server

To run the postgres server

    docker compose up -d

To run the postgres client in attached mode

    docker compose run --rm postgres_client

### User Accounts

Default user `qlik` with default password `qlik123` has superuser permissions to database `qlik`.


### TODO

Add pgadmin service
