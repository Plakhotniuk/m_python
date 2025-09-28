### Создание БД

```shell
docker run -d \
  --name postgres \
  -p 5432:5432 \
  -v $HOME/postgresql/data:/var/lib/postgresql/data \
  -e POSTGRES_PASSWORD=123qwe \
  -e POSTGRES_USER=app \
  -e POSTGRES_DB=movies_database  \
  postgres:16 
```

подключиться к своему серверу Postgres:

```shell
psql -h 127.0.0.1 -U app -d movies_database 
```

Создать БД из .ddl файла:
```shell
psql -h 127.0.0.1 -U app -d movies_database -f movies_database.ddl 
```