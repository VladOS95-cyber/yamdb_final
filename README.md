## API_YamDB

## Description
API for the YamDB project which collects user reviews of works. Works are divided into categories: “Books”, “Movies”, “Music” and implemented based on Django REST_API framework using Python.
A detailed description of requests and data retrieval are located at: http://127.0.0.1:8070/redoc/

## Instructions
An algorithm for registration (by email) and user authentication has been created, and user roles have been added. GET, POST, PATCH, DEL requests are also implemented to obtain or change data in json format.
Clone repo 
```bash
git clone https://github.com/VladOS95-cyber/yamdb_final
```

Docker installation - https://docs.docker.com/docker-for-windows/install/


Run containers
```bash
docker start infra_sp2_db_1, docker start infra_sp2_nginx_1, infra_sp2_web_1
```
Run servers
```bash
CMD python /code/manage.py runserver 0:8070
```
Create superuser
```bash
docker-compose exec web python manage.py createsuperuser
```
Fill database by initial data ./manage.py loaddata fixtures.json

Filling in .env - the project uses a PostgreSQL database, and all the variables necessary to configure a connection to the database are located in the .env file.

Badge - https://github.com/VladOS95-cyber/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg

Project author: Владислав Бронзов
Email: vladislav.bronzov@gmail.com

