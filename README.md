Название проекта - API_YamDB
Краткое описание - API для проекта YamDB (собирает отзывы пользователей на произведения. Произведения делятся на категории: «Книги», «Фильмы», «Музыка».), реализованное на основе REST_API framework. 
Создан алгоритм регистрации(по email) и аутентификации пользователей, добавлены пользовательские роли. Также реализованы запросы GET, POST, PATCH, DEL для получения или изменения данных в форате json. 
Детальное описание запросов и получение данных находятся по адресу: http://127.0.0.1:8070/redoc/
Запуск контейнеров - docker start infra_sp2_db_1, docker start infra_sp2_nginx_1, infra_sp2_web_1
Запуск сервера - CMD python /code/manage.py runserver 0:8070 (прописать последней строкой в Dockerfile)
Команда для создание суперпользователя - docker-compose exec web python manage.py createsuperuser
Команда для заполнения базы начальными данными - ./manage.py loaddata fixtures.json
Бейдж - https://github.com/VladOS95-cyber/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg

Автор проекта: Владислав Бронзов
Почта автора: vladislav.bronzov@gmail.com

