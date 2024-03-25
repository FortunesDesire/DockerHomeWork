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