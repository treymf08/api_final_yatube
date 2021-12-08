В api_yatube реализуеться API для учебного проекта "Yatube".

Проект реализован на Django REST framework.

Как запустить проект:

Клонировать репозиторий :
git clone https://github.com/treymf08/api_final_yatube

Cоздать и активировать виртуальное окружение:
python -m venv venv
source venv/Scripts/activate

Установить зависимости из файла requirements.txt:
python3 -m pip install --upgrade pip
pip install -r requirements.txt

Выполнить миграции:
python3 manage.py migrate

Запустить проект:
python3 manage.py runserver

Примеры запросов к API:

Получение публикаций:
http://127.0.0.1:8000/api/v1/posts/

Получение публикации по id:
http://127.0.0.1:8000/api/v1/posts/{id}/

Получение всех комментариев к публикации:
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/

Получение всех комментариев к публикации:
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/

Получаем все подписки пользователя, сделавшего запрос:
http://127.0.0.1:8000/api/v1/follow/