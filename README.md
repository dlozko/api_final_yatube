### Описание проекта:

Проект api_yatube - это API для социальной сети Yatube.

С помощью api_yatube можно запрашивать данные о постах, группах, комментариях в социальной сети Yatube, а также создавать новые.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/dlozko/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение (выбираем python не ниже 3.7):

```
python -m env venv
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```

### Примеры запросов к API:

Получаем список всех постов (GET):
```
http://127.0.0.1:8000/api/v1/posts/
```

Получаем определенный пост (GET):
```
http://127.0.0.1:8000/api/v1/posts/1/
```

Получаем коментарии определенного поста (GET):
```
http://127.0.0.1:8000/api/v1/posts/1/comments/
```

Получаем список всех групп (GET):
```
http://127.0.0.1:8000/api/v1/groups/
```

Создаем новый пост (POST):

(Требуется аутентификация)
```
http://127.0.0.1:8000/api/v1/posts/
```
