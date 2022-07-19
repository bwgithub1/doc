# Django Heroku  
https://devcenter.heroku.com/articles/getting-started-with-python?singlepage=true#install-app-dependencies-locally
https://realpython.com/django-hosting-on-heroku/
## Steps of deployment
Pre requests
```
Step 1: Scaffold a Django Project for Hosting
-- setup CMD: run -> Ctrl+shit+Enter
	setup VC: Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser (execution policy on PowerShell)	
-- install git
	install herocu CLI
	Creat a free account of Heroku	(https://signup.heroku.com/)
-- virtual environment (cd /path/to/new/virtual/environment)
	1. python -m venv venv
	2. on PS:  venv\Scripts\Activate.ps1
	   on CMD: venv>Scripts\activate.bat
-- django dependences
	python -m pip install --upgrade pip
	python -m pip install django
	python -m pip list (check installed dependences)
	python -m pip freeze (check subfolder detail of dependences)
	
	(encapsulated within one or more requirements files that pip can consume in one go)
	python -m pip freeze > requirements.txt
	python -m pip install -r requirements.txt

-- bootstrap a new Django Project (skip, if a django project was created)
	django-admin startproject portfolio . (method 1, in current root folder)
	python -m django startproject portfolio .  (method 2)
	(for example: under root portfolio-project, management app with name of portfolio)
		portfolio-project/
		├── portfolio/
		│   ├── __init__.py
		│   ├── asgi.py
		│   ├── settings.py
		│   ├── urls.py
		│   └── wsgi.py
		│
		├── venv/
		│
		├── manage.py
		└── requirements.txt
	(start one or more Django apps and define their views and models)

-- Update Local Database Schema (Optional, defaul using SQLite)
	python manage.py migration ???
	python manage.py migrate
-- Run a Local Development Server
	python source/manage.py runserver  (surce is the folder has manage.py)
	http://localhost:8000/admin (admin/superuser) 
	http://localhost:8000 (killbill708@gmail.com/huanghe1   user:mytest)

Step 2: Create a Local Git Repository


	
	-- Use psycopg2-binary instead of psycopg2.
	pip install psycopg2-binary
	
	-- Create three files in the project to be deployed
	(requirements.txt, procfiles and runtime.txt)
	pip install -r requirements.txt
	pip list (list dependances)
	pip freeze > requirements.txt
	
	-- install requests
	python -m pip install requests (pip install requests not work)
	pip install -r requirements.txt
	
	-- ALLOWED_HOSTS
	ALLOWED_HOSTS = ['dry-sands-91151.herokuapp.com' ]
	
Using Heroku CLI (on CMD ternual) type: heroku login
After login, 
on CLI login in Heroku web create new app and follow instruction on new app page
An new applicationi bw_djlogin is created on 7/16/2022

-- start web on local
heroku local -f Procfile.windows
```
#### https://www.youtube.com/watch?v=HgDEFnMV16k
#### https://www.youtube.com/c/LegionScript  (top YouTub)

## Document 
```
Python 3.10.5 doc
	https://docs.python.org/3/
Deploying Django Docs:
	https://devcenter.heroku.com/articles/deploying-python
Configuring Django on Heroku:
	https://devcenter.heroku.com/articles/django-app-configuration
Legion Script:
	https://www.legionscript.com/
https://www.autoscripts.net/deploying-a-django-application-to-heroku-no-module-named-django_project-wsgi/

```
## Sample links

#### Food deliver web site
```	
 07/12/2022
	https://github.com/legionscript/Django-3.2-Series
	https://www.youtube.com/playlist?list=PLPSM8rIid1a0qiCpbfujex5lZoXr2SRFC
Starting Code:
	https://github.com/legionscript/deliver/tree/tutorial6
Ending Code:
	https://github.com/legionscript/deliver/tree/tutorial7
```
## tmp
Creating app... done, ⬢ dry-sands-91151
https://dry-sands-91151.herokuapp.com/ | https://git.heroku.com/dry-sands-91151.git

