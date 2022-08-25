![example event parameter](https://github.com/KuchishkinM/foodgram-project-react/actions/workflows/main.yml/badge.svg?event=push)
[![Python](https://img.shields.io/badge/-Python-464646?style=flat-square&logo=Python)](https://www.python.org/)
[![Django](https://img.shields.io/badge/-Django-464646?style=flat-square&logo=Django)](https://www.djangoproject.com/)
[![Django REST Framework](https://img.shields.io/badge/-Django%20REST%20Framework-464646?style=flat-square&logo=Django%20REST%20Framework)](https://www.django-rest-framework.org/)
[![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-464646?style=flat-square&logo=PostgreSQL)](https://www.postgresql.org/)
[![Nginx](https://img.shields.io/badge/-NGINX-464646?style=flat-square&logo=NGINX)](https://nginx.org/ru/)
[![gunicorn](https://img.shields.io/badge/-gunicorn-464646?style=flat-square&logo=gunicorn)](https://gunicorn.org/)
[![docker](https://img.shields.io/badge/-Docker-464646?style=flat-square&logo=docker)](https://www.docker.com/)
[![GitHub%20Actions](https://img.shields.io/badge/-GitHub%20Actions-464646?style=flat-square&logo=GitHub%20actions)](https://github.com/features/actions)
[![Yandex.Cloud](https://img.shields.io/badge/-Yandex.Cloud-464646?style=flat-square&logo=Yandex.Cloud)](https://cloud.yandex.ru/)
# Приложние Foodgram
Ссылка на проект: http://84.201.139.93/
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