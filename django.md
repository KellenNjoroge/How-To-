# Creating a Virtual env (do once)

** $ python3.6 -m venv --without-pip virtual

## Activating a virtual env

 ** source virtual/bin/activate

## Install latest version of pip

 ** (virtual)$ curl https://bootstrap.pypa.io/get-pip.py | python

## Deactivate virtual env

 ** $ deactivate

## Downloading django

** (virtual)$ pip install django==1.11

## creating a django project 

** (virtual)$ django-admin startproject < projectname > .

--- create app which is submodule of project

** django-admin startapp < appname >

** python manage.py createsuperuser
