# Проект Yatube

<i>В данном проекте был реализован бекенд и фронтенд веб-сайта позволяющего пользователям проходить регистрацию, создавать новые записи, оставлять комментарии и подписываться на других пользователей.</i>

<i><b>Шаблон наполнения env-файла:</i></b><br>
<i>
DB_ENGINE=указываем, что работаем с postgresql<br>
DB_NAME=имя базы данных<br>
POSTGRES_USER=логин для подключения к базе данных<br>
POSTGRES_PASSWORD=пароль для подключения к БД (установите свой)<br>
DB_HOST=название сервиса (контейнера)<br>
DB_PORT=порт для подключения к БД<br>
SECRET_KEY = Секретный ключ</i><br>


<i><b>Описание команд для запуска приложения в контейнерах:</i></b><br>
<i>
'docker-compose up' - Запускаем docker-compose<br>
'docker-compose exec web python manage.py migrate' - Делаем миграции<br>
'docker-compose exec web python manage.py createsuperuser' - Создаем суперпользователя<br>
'docker-compose exec web python manage.py collectstatic' --no-input =Собираем статику<br>
По адресу <http://localhost/admin/> открывается админка, введите логин и пароль, которые указывали при создании пользователя<br>
'docker-compose exec web python manage.py dumpdata > fixtures.json' - команда для создание резервной копии базы <br>
'docker-compose down -v'= Команда чтобы остановить контейнеры </i>
</li>
<i><b>Технологии</i></b>
<blockquote>
☑ Python 3.7.0 <br>
☑ Django
☑ Docker
</blockquote>

Авторы:
<b>Дмитрий Венде</b><br>
![branch parameter](https://github.com/Vende1337/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)