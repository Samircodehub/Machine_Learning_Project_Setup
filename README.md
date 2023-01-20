# Machine_Learning_Project_Setup

## Start Machine Learning project.
##### Software and account Requirement.
1. Github Account
2. Heroku Account
3. VS Code IDE
4. GIT cli
5. GIT Documentation
6. Creating conda environment
7. CICD Tool :Github Action (In github)

* conda create -p InterpreterName python==3.9 -y
* conda activate venv/
* OR

* conda activate venv
* pip install -r requirements.txt

#### To setup CI/CD pipeline in heroku we need 3 information

1. HEROKU_EMAIL = 
2. HEROKU_API_KEY = <>
3. HEROKU_APP_NAME = ml-regression-app

Dockerfile:
1. which operating system as base layer in docker image i.e. python:3.9
2.  copy all the code from currunt directory in app folder
3. To change directory as "app" as working directory
4. install requirments.txt which is copied inside app folder
5. Port: port is a envirment variable (It is not specified here, This port value will be supplied by Heroku during deployment). 4 workers means there will be 4 listener for web server eg. if there are 1000 reuest comming then all request will be handled like 250 250 250 250,so work to handle will done fast
Gunicorn is a simple web server get way interface which help to handle web server request 
6. command to launch application i.e. gunicorn with local host ip address(0.0.0.0), file_name(Module):application object_name


#### setup file:
setup() is pre built function 
setup file used to installing libraries  using coding insted of using pip install requirement.txt
#### housing
__init__py file is like a creating library which we are creating and which we can import. Inside housing we are going to create packages

##### packages 
It will return all all folders in which __init__py is exist and then it will try to install package(housing)
Those folder which have __init__py that we call package

Apart from above packages we need other external libraries tgat we specified in reuirements.txt file which will also installed.

##### Inside housing folder
Inside housing folder we are going to craete folders as packages that will help to smoothing the project process
1. creating exception handeling package
2. creating logger package 
3. pipeline 
4. component (stages)
4. config
5. entity
* step1: create all above file inside housing folder and __init__py file in each folder so that ach folder act like package

 * Step2: build code in ecah folder
       * logger file: to track all process of running code maeans what happening
       * exception file:  to handle exceptoin handeling
         - Traceback: It gives us file name as well as line number where error is occured during run  [exe.info()]