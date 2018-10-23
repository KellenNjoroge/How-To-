# DEPLOYING TO HEROKU

## Install gunicorn 

(virtual)$ python3.6 -m  pip install gunicorn

## Create a free Heroku account

## Install heroku CLI

$ sudo snap install --classic heroku
            or 
    $ curl https://cli-assets.heroku.com/install.sh | sh
Check heroku version
    $ heroku --version
Access heroku database 
    $ heroku psql --app <appname>

## GETTING STATED WITH HEROKU

$ heroku login
$ cd ~/myapp

(virtual)$ pip freeze > requirements.txt
(virtual)$ heroku login
(virtual)$ heroku create <name-of-app>

heroku config:set   -API_KEY <YOUR API KEY>
                    -SECRET_KEY<YOUR SECRET KEY>
                    -MAIL_USERNAME
                    -MAIL_PASSWORD
Heroku addons :create heroku postgresql
Add database URI to config.py
    (virtual)$ pip freeze > requirements.txt
    (virtual)$ git push heroku master
    (virtual)$ heroku run python3.6 manage.py db upgrade

## how to see logs from CLI

heroku logs -t
