# The Road Home Volunteer Time Tracker
https://road-home.herokuapp.com

## Install Python
Download and install python 3.6.1
https://www.python.org/downloads/

Install using defaults and add it to your path with windows installer or Linux env variable

## Use bash or PowerShell to find if pip is installed
Open bash or PowerShell (ps) and type
> pip --version

to make sure you have version v9.0.1

We will use pip to download and install all the packages needed. You'll need the .env file to build locally. You have that file if you are a contributor to the project. This will hold passwords and secrets that are not shared online. Please do not ever commit it. It's already in the .gitignore file and as long as it remains there, we never have to worry.

## Clone the repo
First download this repo and then browse to it in bash or ps and

## Install virtualenv
type into ps or bash:
> pip install virtualenv

to install the latest version of virtualenv and now you need to set it up
> virtualenv venv

## Install postgres
After which, install postgres locally using this: https://www.enterprisedb.com/downloads/postgres-postgresql-downloads and using the latest version v9.6.3 and use a good password and remember it. **NEVER commit it!**

## Sometimes not required, you'll have to test
Remember to update your PATH environment variable to add the bin directory of your Postgres installation. The directory will be similar to this: C:\Program Files\PostgreSQL\<VERSION>\bin. If you forget to update your PATH, commands like heroku pg:psql won’t work.

# Enable VENV - ALWAYS BEFORE WORKING
Enable venv in the directory with powershell/cmd
> .\venv\Scripts\activate

and for Linux bash
> source .\venv\bin\activate

## Install pip requirements - EVERY GIT PULL
Then type
> pip install -r requirements.txt

and watch the downloads go by. This installs all the requirements you need to run the website. Congrats! Way easier than PHP…

## Run locally - FOR TESTING
> python manage.py runserver

## View in Browser
http://localhost:8000

### Training
I recommend using CodeSchool to know how Django and python work
https://www.codeschool.com/courses/try-django

Link to Django's tutorial:
https://docs.djangoproject.com/en/1.11/intro/tutorial01/
