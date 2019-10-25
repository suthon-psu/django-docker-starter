**How to start
>> docker-compose up


**How to execute command
>> docker exec -it dj-web python manage.py xxx


** When requirements.txt changed
>> docker rm dj-web
>> docker rmi dj-web

** create admin
>> docker exec -it dj-web python manage.py createsuperuser --email admin@bonmek.com --username admin


** update model
##docker exec -it dj-web python manage.py makemigrations <model>
docker exec -it dj-web python manage.py migrate

** This project is initialized using
docker-compose run web django-admin startproject dj_web .