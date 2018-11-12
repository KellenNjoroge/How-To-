# DB HOW TO

## Installing postgress

-- First get required updates
** $ sudo apt-get update

## Install postgress

**  $ sudo apt-get install postgresql postgresql-contrib libpq-dev

## Create super user

** $ sudo -u postgres createuser --superuser $USER
--Have your username
**$ sudo -u postgres createdb $USER
--Save your history
** $ touch .psql_history
-- PSQL terminal 
** $ psql
--quit PSQL terminal
** $ \q

## Create DB Flask

** CREATE DATABASE < databasename >;

## Create password

dbname=# ALTER USER kellen password 'new password';

## See your password

** $  \password

## DJANGO DB-HOW TO

** install dependency

(virtual)$ pip install psycopg2

** create database
(virtual)$ psql
kellen=# CREATE DATABASE tribune;

** Configurations

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': '< databasename >',
        'USER': '< Your Database Username >',
    'PASSWORD':'< Your Database Password >',
    }
}

** setting time zone

TIME_ZONE = 'Africa/Nairobi'

** migrations

(virtual)$ python3.6 manage.py migrate

** make migrations

python manage.py makemigrations < djangoappname >

** view migrations

(virtual)$ python3.6 manage.py sqlmigrate < djangoappname > 0001

** run migrations

python3.6 manage.py migrate

heroku

heroku pg:reset 

heroku pg:push tribune DATABASE_URL --app kellerstribune

