# Металлография

Приложение для конвертации изображений электронного микроскопа в размеченные.

https://youtu.be/_xVUbHiFV3Y

<iframe width="560" height="315" src="https://www.youtube.com/embed/_xVUbHiFV3Y" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Приложение содержит в себе обученную на размеченных специалистами изображениях нейросетевую модель.

Модель собирали при помощи сервиса https://liner.ai/.

Модель тестировали в тетрадке https://www.kaggle.com/code/eavprog/liner-keras-model-1000-tr25-test5.


# Сборка образа сервера

Загрузите к себе папку с проектом командой в терминале (если у вас нет установленного `git`, перейдите по ссылке https://git-scm.com/ и установите у себя):
```
git clone https://github.com/prog815/fraktMetal.git
```
Появится папка `fraktMetal`. Перейдите в эту папку.
Запустите сборку образа командой (если у вас нет установленного `Docker` перейдите по ссылке https://www.docker.com/products/docker-desktop/ и установите):
```
docker-compose build
```
# Запуск сервера
Находясь в паке проекта запустите команду:
```
docker-compose up -d
```
Проверяем статус работы сервера командой в терминале:
```
docker-compose ps -a
```
Должен работать контейнер `app` из образа `fraktmetal-app`.
# Открываем программу

![Alt text](image-1.png)

Для доступа к интерфейсу программы откройте в браузере адрес http://localhost:8000/.

# Удаление образа и проекта
Останавливаем сервер по команде в терминале:
```
docker-compose down
```
Удаляем образ сервера по команде в терминале:
```

```

На всякий пожарный случай полная очистка неиспользуемых контейнеров:
```
docker system prune --all --force
```

