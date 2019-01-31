# DjangoDocker
A Django Sample App in Docker

Based on https://docs.djangoproject.com/en/2.1/intro/tutorial01/

a -> Install Python and make sure C:\Pythonxx-xx and C:\Pythonxx-xx\Scripts are in your path
b -> Install pip if you are using winwdows this will be
	python -m pip install -U pip
c -> Install virtualenv
	pip install virtualenv
d -> Create a virtualenv
	py -m virtualenv env
e -> Install Django
	pip install Django
f -> Check your django version
	python -m django --version

	Mine is 2.1.5

g -> Creating a project
	django-admin startproject sampleapp

h -> Verify Django project works
	python manage.py runserver

i -> docker build . -t architectednet/django-app

j -> docker run -d -p 8001:8000/tcp --name my-django-container architectednet/django

k -> docker port my-django-container

l-> navigate to http://localhost:8001/polls
