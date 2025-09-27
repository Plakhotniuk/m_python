### Запустить сервисы можно командой 

```shell
docker compose up -d
```


### Полезные команды:

```shell
docker compose  stop  # остановить все сервисы.
docker compose  rm  # удалить все сервисы.
docker compose  down  # остановить и удалить все сервисы.
docker compose  restart  # перезапустить все сервисы.
docker compose  build  # пересобрать все использующиеся образы.
docker compose  exec backend ls  # посмотреть, какие файлы есть в контейнере
```
