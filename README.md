# DockerHomeWork
Internal course homework

Сборка образа
```
docker build -t weatherapp_homework2 -f Dockerfile.hw .
```

Запуск контейнера с пробросом порта
```
docker run -d -p 5000:80 --name weatherapp-app weatherapp_homework2
```

Проверить, что сервис отвечает на эндпоинте /weatherforecast
```
http://localhost:5000/weatherforecast
```

# ------------------------------
Домашняя работа 3:

Был создан файл docker-compose.yml, описывающий образ приложения в формате yml.

Запуск всех образов в директории в бекграунде
```
docker-compose up -d
```

# -----------------------------
Домашняя работа 4:

Сформированы конфигурационные файлы для нжинкса и для сервиса погоды в формате, подходящем для Docker swarm

Запуск контейнера:
```
docker stack deploy -c docker-stack.yml weather-app
```
