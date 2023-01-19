# Machine_Learning_Project_Setup

## Start Machine Learning project.
##### Software and account Requirement.
1. Github Account
2. Heroku Account
3. VS Code IDE
4. GIT cli
5. GIT Documentation
6. Creating conda environment

* conda create -p InterpreterName python==3.9 -y
* conda activate venv/
* OR

* conda activate venv
* pip install -r requirements.txt

#### To setup CI/CD pipeline in heroku we need 3 information

1. HEROKU_EMAIL = samirpmendhe@gmail.com
2. HEROKU_API_KEY = <>
3. HEROKU_APP_NAME = ml-regression-app

Dockerfile:
1. which operating system as base layer in docker image i.e. python:3.9
2.  copy all the code from currunt directory in app folder
3. To change directory as "app" as working directory
4. install requirments.txt which is copied inside app folder
5. Open port: port is a envirment variable
6. command to launch application i.e. gunicorn with local host ip address(0.0.0.0), file_name:application object_name


