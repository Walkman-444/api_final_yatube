# Проект «API для Yatube»
Yatube это социальная сеть, в которой пользователи могут создовать посты и группы, добавлять фотографии, подписываться друг на друга.
API для Yatube является приложением для взаимодействия и обмена данными с другими API.

## Технологии и запуск проекта
Проект написан на языке python, с использованием django REST framework.
#### Технологии проекта:
- Python 3.7
- Django 3.2.16
- Django Rest Framework 3.12.4
- API REST
- Simple-JWT
#### Запуск проекта:
- клонируйте репозиторий
```
    git clone https://github.com/Walkman-444/api_final_yatube
```
- создайте и активируйте виртуальное окружение
```
python -m venv venv
source venv/scripts/activate
```
- установите необходимые зависимости
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```
- выполните миграции
```
python manage.py makemigrations
python manage.py migrate
```
- запустите проект
```
python manage.py runserver
```
## Работа в проекте
##### Документация для проекта «API для Yatube» доступна по адресу http://127.0.0.1:8000/redoc/
#### Примеры эндпоинтов:
##### GET запросы
```
- http://127.0.0.1:8000/api/v1/posts/ - Получение побликаций
- http://127.0.0.1:8000/api/v1/posts/{id}/ - Получение побликации
- http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/ - Получение комментариев
- http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/ - Получение комментария
- http://127.0.0.1:8000/api/v1/groups/ - Список сообществ
- http://127.0.0.1:8000/api/v1/groups/{id}/ - Информация о сообществе
- http://127.0.0.1:8000/api/v1/follow/ - Подписки
```
##### POST запросы:
```
- http://127.0.0.1:8000/api/v1/posts/ - Создание публикации
- http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/ - Добавление комментария
- http://127.0.0.1:8000/api/v1/follow/ - Подписка
- http://127.0.0.1:8000/api/v1/jwt/create/ - Получить JWT-токе
- http://127.0.0.1:8000/api/v1/jwt/refresh/ - Обновить JWT-токен
- http://127.0.0.1:8000/api/v1/jwt/verify/ - Проверить JWT-токен
```
##### PUT запросы:
```
- http://127.0.0.1:8000/api/v1/posts/{id}/ - Обновление публикации
- http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/ - Обновление комментария
```
##### PATCH запросы:
```
- http://127.0.0.1:8000/api/v1/posts/{id}/ - Частичное обновление публикации
- http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/ - Частичное обновление комментария
```
##### DEL запросы:
```
- http://127.0.0.1:8000/api/v1/posts/{id}/ - Удаление публикации
- http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/ - Удаление комментария
```
## Автор
Иванов Максим - студент Яндекс Практикум. Курс Python-разработчик
