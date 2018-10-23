# INSTALLING FLASK

## Creating a Virtual env (do once)

** $ python3.6 -m venv --without-pip virtual

## Activating a virtual env

 ** source virtual/bin/activate

## Install latest version of pip

 ** (virtual)$ curl https://bootstrap.pypa.io/get-pip.py | python

## Deactivate virtual env

 ** $ deactivate

## copy pasting to requirements.txt

** pip freeze > requirements.txt

### Installing from  requirements.txt

** (virtual)$ pip install -r requirements.txt

## Do it inside virtual env

 ** $ pip install Flask

## Install bootstrap

** (virtual)$ pip install Flask-Bootstrap
Install WTF forms
** (virtual)$ pip install Flask-Wtf
Install JWT(for security)
** (virtual) pip install Flask-JWT
Install flask script
** (virtual) pip install Flask-Script
Install SQLalchemy
** pip install Flask-SQLAlchemy
** pip install gunicorn

## For Migrations

** (virtual) $ pip install Flask-Migrate
** (virtual) pip install Flask-Psycopg2

## For Authentication and loging in

** (virtual) $ pip install Flask-Login
To enable flask-uploads
** pip install Flask-Uploads

## To enable SMTP

** pip install Flask-Mail

## To convert markdown to HTML

** pip install flask_markdown2
** pip install flask-simplemde markdown2

## Install everything required

**(virtual) pip install -r requirements.txt

## LARGE APP STRUCTURE(noSQL)

    |-Root_Folder
    |-app/
        |-main/
            |-__init__.py
            |-errors.py
            |-forms.py
            |-views.py
        |-static/
            |-css
            |-js
            |-photos
        |-templates/
            |-index.html
            |-macros.html
            |-navbar.html
            |-base.html
            |-404.html
        |-__init__.py
        |-models.py
        |-requests.py
    |-instance
        |- __init__.py
        |- config.py
    |-tests/
    |-virtual/
    |-config.py
    |-.gitignore
    |-LICENSE
    |-Procfile
    |-README.md
    |-specs.md
    |-manage.py
    |-requirments.txt
    |-runtime.txt
    |-start.sh


## LARGE APP STRUCTURE(SQL)

    |-Root_Folder
    |-app/
        |-auth
            |-__init__.py
            |-forms.py
            |-views.py
        |-main/
            |-__init__.py
            |-errors.py
            |-forms.py
            |-views.py
        |-static/
            |-css
            |-js
            |-photos
        |-templates/
            |-auth/
                |-change_password.html
                |-Login.html
                |-register.html
                |-reset.html
                |-reset_password.html
                |-reset_password.txt
            |-Profile/
                |-profile.html
                |-update.html
            |-index.html
            |-macros.html
            |-navbar.html
            |-base.html
            |-404.html
        |-__init__.py
        |-models.py
        |-requests.py
    |-Migrations
    |-tests/
    |-virtual/
    |-config.py
    |-.gitignore
    |-LICENSE
    |-Procfile
    |-README.md
    |-specs.md
    |-manage.py
    |-requirements.txt
    |-runtime.txt
    |-start.sh