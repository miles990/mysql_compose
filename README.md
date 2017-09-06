# Easy to Connect MySQL Environment

## Required
- Docker Compose[Get Docker Community Edition](https://www.docker.com/community-edition)

## How to use ?
- cd to directory
- Execute `./run.sh`

## Connect to MySQL
- `docker-compose exec mysqlDb mysql -u user_name -h localhost -p'user_password'`

## Dump from MySQL
- `docker-compose exec mysqlDb mysqldump -u user_name -h localhost -p'user_password --all-databases > backup/dump_all.sql'`

## Restore to MySQL
- `docker-compose exec mysqlDb mysql -u user_name -h localhost -p'user_password < backup/dump_all.sql'`