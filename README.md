# compose-mysql

Docker Compose using Docker Hub [Postgres](https://hub.docker.com/_/postgres)


### Running Server

To run the postgres server

    docker compose up -d

To run the postgres client in attached mode

    docker compose run --rm postgres_client

To run [adminer](https://hub.docker.com/_/adminer)

    docker compose --profile admin up -d

Adminer (formerly phpMinAdmn) will run on a dynamically assigned port.
You can get the dymamic port from the docker desktop gui, or use docker inspect:

    docker inspect --format '{{ (index .NetworkSettings.Ports "8080/tcp" 0).HostPort }}' <adminer_container_name>

### User Accounts

Default user `qlik` with default password `qlik123` has superuser permissions to database `qlik`.


### TODO

Add pgadmin service
