# 📑 Recipe API
Recipe App API project

## 📝 Linting
Run linting on the project

    docker-compose run --rm app sh -c "flake8"


## 🧪 Testing
Command to run the tests localy

    docker-compose run --rm app sh -c "python manage.py test"

## 🐘 Database commands
Creating Migrations for database

    docker-compose run --rm app_name sh -c "python manage.py makemigrations"

Apply Migrations to database

    docker-compose run --rm app -sh -c "python manage.py migrate"

Check availabiloty of the postgres service

    docker-compose run --rm app sh -c "python manage.py wait_for_db"

Clear our data for the database

    docker volume rm name_of_the_volume

## 🐋 Util Docker commands
Build our Docker Image

    docker-compose build

Start our services

    docker-compose up

List our volumes

    docker volume ls

Clear all the container that we are using

    docker-compose down