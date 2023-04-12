# Микросервисная архитектура с NestJS, RabbitMQ и PostgreSQL


## Работа с Docker и docker-compose

Запуск всех сервисов 
```
docker-compose up
```

Очистка всех сервисов (удаление контейнеров) 
```
docker-compose down
```

Если в `package.json` были добавлены новые зависимости, то недостаточно запустить сервисы или пересобрать образы. Необходимо указать ключ для игнорирования кэша чтобы обновить пакеты у сервиса.
```
docker-compose build --no-cache [<service_name>..]
```

---


