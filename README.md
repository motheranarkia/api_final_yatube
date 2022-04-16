____

# Проект «API для Yatube»
____

## Для чего нужен проект? 

Создание API сервиса для авторского блогинга с возможностью создавать посты, комментировать посты, создавать тематические группы, подписываться на понравившихся авторов.

## Как запустить проект:

Склонируйте репозиторий:

```
git clone git@github.com:motheranarkia/api_final_yatube.git
```

Активируйте виртуальное окружение и установите зависимости из файла __requirements.txt__:

```
python -m pip install

pip install -r requirements.txt
```
Выполните миграции:
```
python manage.py migrate
```
Запустите проект:
```
python manage.py runserver
```
## Примеры использования:

Получить список всех постов:
```
GET /api/v1/posts/
```
Добавление нового поста:
```
POST /api/v1/posts/
```
Получить список всех групп:
```
GET /api/v1/groups/
```
Добавление нового комментария:
```
POST /api/v1/posts/{post_id}/comments/
```
Удаление комментария по id:
```
DELETE /api/v1/posts/{post_id}/comments/{id}/
```
Получение списка подписок:
```
GET /api/v1/follow/
```
Подписка пользователя на пользователя переданного в запросе:
```
POST /api/v1/follow/
```
## Используемые технологии

+ Python 3.9
+ Django==2.2.16

## А кто же автор?

Анна :penguin:
Python-разработчик 
+ [GitHub](https://github.com/motheranarkia)
