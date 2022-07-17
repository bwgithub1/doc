# Django Heroku  
https://devcenter.heroku.com/articles/getting-started-with-python?singlepage=true#install-app-dependencies-locally
## Steps of deployment
Pre requests
```
Pre requests
	install git
	install herocu CLI
	Creat a free account of Heroku	(https://signup.heroku.com/)
	
	--setting the execution policy for the user ( on PowerShell)
	Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
	
	-- python3 -m venv /path/to/new/virtual/environment 
	-- (a common name for the target directory is .venv)
	python -m venv venv
	-- To be “activated” C:\> <venv>\Scripts\activate.bat
	-- (<venv> must be replaced by the path of the directory containing the virtual environment) 
	-- PS
	C:\dev\gitlocal\python-getting-started\venv\Scripts\Activate.ps1
	--CMD
	C:\dev\gitlocal\python-getting-started\venv>Scripts\activate.bat
	
	-- make pip update
	python -m pip install -U pip
	
	-- Use psycopg2-binary instead of psycopg2.
	pip install psycopg2-binary
	
	-- Create three files in the project to be deployed
	pip install -r requirements.txt
	pip list (list dependances)
	pip freeze > requirements.txt
	
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

