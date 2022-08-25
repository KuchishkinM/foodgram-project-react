![example event parameter](https://github.com/KuchishkinM/foodgram-project-reac
/actions/workflows/main.yml/badge.svg?event=push)
# Приложние Foodgram
## Описание

Это продуктовый помощник, который дает возможность:
* Создавать рецепты
* Подписываться на авторов рецептов
* Добавлять рецепты других пользователей в избранное
* Формировать и скачивать список покупок

### Установка проекта:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/KuchishkinM/foodgram-project-react
cd foodgram-project-react
```
Перейти в папку infra и создать там файл .env и заполнить его по примеру:
```
cd infra
touch .env
```
Примерное содержание файла .env

```
DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
DB_HOST=db
DB_PORT=5432
```
### Запуск проекта на сервере:

Установить Docker и Docker-compose:

```
sudo apt install docker.io
sudo apt install docker-compose
```

Выполнить миграции:

```
sudo docker-compose exec backend python manage.py migrate
```

Создать суперпользователя:

```
sudo docker-compose exec backend python manage.py createsuperuser
```
Собрать статику:

```
sudo docker-compose exec backend python manage.py collectstatic --no-input
```
### Автор: Кучишкин Максим