# Установка

Установить python-модуль jinja2.

Переименовать `config.py.ex` в `config.py`, прописать настройки.

## nginx

```
server {
    listen 80;
    server_name yourdomain;
    location / {
            root   /path/to/www;
            index  index.html;
    }
}
```

## crontab

```
12 4 * * * /usr/bin/python /path/to/www/generate.py >> /path/to/www/cron-run.log 2>&1
```