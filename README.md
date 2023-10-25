# проект по фрактографии

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

Для доступа к интерфейсу программы откройте в браузере адрес http://localhost:8000/.

# Удаление образа и проекта
Останавливаем сервер по команде в терминале:
```
docker-compose down
```
Удаляем образ сервера по команде в терминале:
```

```

