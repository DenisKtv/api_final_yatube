# API_FINAL_YATUBE
##### API_Final - законченная версия API для yatube.
##### Стек: Python 3.7, Django Rest Framework, SQLite
## Как запустить проект:

- Клонировать репозиторий и перейти в него в командной строке:
``` sh
https://github.com/Imbalanser/api_final_yatube.git
```
- Cоздать и активировать виртуальное окружение:
``` sh
python3 -m venv env
source venv/bin/activate
```
- Установить зависимости из файла requirements.txt:
``` sh
python3 -m pip install --upgrade pip
pip install -r requirements.txt
```
- Выполнить миграции:
``` sh
python3 manage.py migrate
```
- Запустить проект:
``` sh
python3 manage.py runserver
```
## Примеры запросов:
``` sh
GET: http://127.0.0.1:8000/api/v1/posts/
[
    {
        "id": 1,
        "author": "Anton",
        "image": null,
        "text": "Все тлен",
        "pub_date": "2022-10-08T06:41:23.744402Z",
        "group": null
    }
]
```
``` sh
GET: http://127.0.0.1:8000/api/v1/groups/
[
    {
        "id": 1,
        "title": "Рок",
        "slug": "rocks",
        "description": "all about rock"
    },
    {
        "id": 2,
        "title": "Кино",
        "slug": "films",
        "description": "all about cinema"
    }
]
```
