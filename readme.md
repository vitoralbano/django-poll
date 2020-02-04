# Django Polls tutorial
This project consists on Django's, a python framework, introduction tutorial, "Writing your first Django app". It is available in Django's documentation, at tutorial section, and you can access it [here](https://docs.djangoproject.com/en/3.0/intro/tutorial01/). As it was for learning purpose, I decided to use SQLite to hold my data, but of course, it's not recommended for production environment.

## Requirements
* pip
* pipenv with python 3 to create a virtual environment and install dependencies. 

To know more about pipenv and for why it is used, check the article ["Pipenv: A Guide to the New Python Packaging Tool"](https://realpython.com/pipenv-guide/) at the Real Python web site.

## How to run
Before it begins, be certain that you have python 3 and pip installed, if you don't, see how to install them in [python](https://www.python.org/downloads/) and [pipenv](https://pypi.org/project/pipenv/) at your environment.

1. Clone the project
```shell
git clone git@github.com:vitoralbano/django-poll.git
```
2. Enter in the project folder and install the dependencies:
```shell
cd django-poll
pipenv install
```
3. Activate the virtual environment:
```shell
pipenv shell
```
4. To create any necessary database tables, go inside 'polls' app folder and run the migrations.
```shell
cd basic-poll
python manage.py migrate
```
5. To create a superuser, project's admin, run the command below and fill the required fields as you wish:
```shell
python manage.py createsuperuser
```
6. Run the development server:
```shell
python manage.py runserver
```
7. Great! At this point just access:
    * Administration panel at: http://localhost:8000/admin/
    * Navigate and vote polls at: http://localhost:8000/polls/
