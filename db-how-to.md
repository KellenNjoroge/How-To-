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

## Create DB

** CREATE DATABASE <databasename>;

## Create password

dbname=# ALTER USER kellen password 'new password';

## See your password

** $  \password
