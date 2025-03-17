# Django REST API Project

## Описание

Это проект Django REST API с использованием SQLite в качестве базы данных.

## Установка и запуск

1. Убедитесь, что у вас установлен [Docker](https://www.docker.com/get-started) и [Docker Compose](https://docs.docker.com/compose/install/).

2. Перейдите в необходимую директорию
```
    cd /api_with_restrictions/
```

3. Соберите образ и запустите контейнер:

```
    docker-compose up --build
```
   

4. Откройте браузер и перейдите по адресу http://localhost:8000, чтобы увидеть ваш сервер.

5. Для остановки контейнера используйте:

   
```
   docker-compose down
```
   

## Примечания

- Все изменения в коде будут автоматически отражаться в контейнере благодаря тому, что мы монтируем текущую директорию в /app.