## Пример работы с web-server

### Запуск сервера приложений:

1) uWSGI
```shell
uwsgi --http :8001 --module my_server:hello
```

2) Gunicorn

```shell
PORT=8002 gunicorn my_server:hello
```

### Запуск Django c uWSGI

Запуск uWSGI-сервера базовыми настройками:
```shell
uwsgi --module=config.wsgi --http :8000
```

Запуск uWSGI-сервера с кастомными настройками:
```shell
uwsgi --ini uwsgi.ini
```

