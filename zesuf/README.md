# Zesuf

The project has three basic apps:

* Feed (A Twitter-like microblog)
* Articles (A collaborative blog)
* Question & Answers (A Stack Overflow-like platform)

## Feed App

The Feed app has infinite scrolling, activity notifications, live updates for likes and comments, and comment tracking.


## Articles App

The Articles app is a basic blog, with articles pagination, tag filtering and draft management.


## Question & Answers App

The Q&A app works just like Stack Overflow. You can mark a question as favorite, vote up or vote down answers, accept an answer and so on.


## Technology Stack

- Python 2.7 / 3.5
- Django > 1.9
- Twitter Bootstrap 3
- jQuery 2


## Installation Guide

Installing and Running Zesuf

1 Install Python 2.7 and Django Framework 1.9

Python 2.7.x https://www.python.org/downloads/

Django 1.9.x https://docs.djangoproject.com/en/1.9/intro/install/

2 Clone the repository

Via https

git clone https://github.com/vitorfs/bootcamp.git
or via ssh

git clone git@github.com:vitorfs/bootcamp.git
3 Install dependencies

On the project root there is a requirements.pip file. Make sure you install all the required dependencies before running Bootcamp

pip install -U -r requirements.txt
Note: If you are having problems with Pillow installation please take a look on a detailed installation guide at: http://pillow.readthedocs.org/en/latest/installation.html

4 Python Decouple

As the project uses python-decouple you will need to create a file named .env on the root of the project with three values, as following:

DEBUG=True
SECRET_KEY='mys3cr3tk3y'
DATABASE_URL='postgres://u_bootcamp:p4ssw0rd@localhost:5432/bootcamp'
Note: You can use Django methods to create a new SECRET_KEY https://github.com/django/django/blob/master/django/core/management/commands/startproject.py

Note 2: To use sqlite on development environment you can change the DATABASE_URL to something like 'sqlite:////Users/vitorfs/Development/bootcamp/db.sqlite3

5 Syncdb

python manage.py migrate
6 Run

python manage.py runserver


