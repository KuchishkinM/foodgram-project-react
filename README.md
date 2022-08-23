# Приложние Foodgram
## Описание

Это продуктовый помощник, который дает возможность:
* Создавать рецепты
* Подписываться на авторов рецептов
* Добавлять рецепты других пользователей в избранное

## Документация 

http://localhost/api/docs/

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
DB_NAME=foodgram
POSTGRES_USER=kmc
POSTGRES_PASSWORD=842764
DB_HOST=127.0.0.1
DB_PORT=5432
```
### Запуск проекта:
Перейти в директорию с файлом manage.py:
```
cd ..
cd backend/foodgram
```
Запустить локальный сервер:
```
python manage.py runserver
```
### Автор: Кучишкин Максим