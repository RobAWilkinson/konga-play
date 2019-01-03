# Kong and Konga Demo

## Instructions

* Create the DB with `docker-compose run kong-database psql -h kong-database -U kong -c "create database konga;" kong`
* Prepare the db with `docker-compose run konga -c prepare -a postgres -u postgresql://kong@kong-database:5432/konga`
* start things with `docker-compose up`
* konga UI available at `http://localhost:1337`
* attach to kong via `http://kong:8001`