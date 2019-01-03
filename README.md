# Kong and Konga Demo

## Instructions

* Migrate the DB with `docker-compose run kong kong migrations up`
* Prepare the db with `docker-compose run konga -c prepare -a postgres -u postgresql://kong@kong-database:5432/kong`
* start things with `docker-compose up`
* konga UI available at `http://localhost:1337`
* attach to kong via `http://kong:8001`