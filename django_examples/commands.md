### Основа для конфигурации проекта

```shell
django-admin startproject config .
```

### Запуск сервера в режиме разработки
```shell
python manage.py runserver
```

manage.py — консольная утилита для управления созданным проектом.

Генерация секретного ключа в терминале:
```shell
python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"
```