#The Road Home Volunteer Time Tracker

##Install Python
Download and install python 3.6.1
https://www.python.org/downloads/

Install using defaults and add it to your path with windows installer or Linux env variable

##Use bash or PowerShell
Open bash or PowerShell (ps) and type pip --version to make sure you have version v9.0.1

We will use pip to download and install all the packages needed. You'll need the .env file to build locally. You have that file if you are a contributor to the project. This will hold passwords and secrets that are not shared online. Please do not ever commit it. It's already in the .gitignore file and as long as it remains there, we never have to worry.

##Clone the repo
First download this repo and then browse to it in bash or ps and type 'pip install virtualenv' to install the latest version.

##Install postgres
After which, install postgres locally using this: https://www.enterprisedb.com/downloads/postgres-postgresql-downloads and using the latest version v9.6.3 and use a good password and remember it. NEVER commit it!

##Sometimes not required, you'll have to test
Remember to update your PATH environment variable to add the bin directory of your Postgres installation. The directory will be similar to this: C:\Program Files\PostgreSQL\<VERSION>\bin. If you forget to update your PATH, commands like heroku pg:psql won’t work.

#Enable VENV
Enable venv in the directory with bash or ps open: .\venv\Scripts\activate for windows and source .\venv\Scripts\activate for bash

##Install pip requirements
Then type 'pip install -r requirements.txt' and watch the downloads go by. This installs all the requirements you need to run the website. Congrats! Way easier than PHP…

##Run locally
python manage.py runserver

##View in Browser
http://localhost:8000
