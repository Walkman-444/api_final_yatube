# Проект «API для Yatube»
## Технологии и запуск проекта
Проект написан на языке python, с использованием django REST framework.
#### Технологии проекта:
- Python
- Django Rest Framework

Документация для проекта «API для Yatube» доступна по адресу http://127.0.0.1:8000/redoc/
#### Запуск проекта:
- клонируйте репозиторий
git clone https://github.com/Walkman-444/api_final_yatube
- создайте и активируйте виртуальное окружение
python -m venv venv
source venv/scripts/activate
- установите необходимые зависимости
python -m pip install --upgrade pip
pip install -r requirements.txt
- выполните миграции
python manage.py makemigrations
python manage.py migrate
- запустите проект
python manage.py runserver