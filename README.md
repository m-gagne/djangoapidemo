# README

Just a testing place for learning Django REST API & Azure AD

## Dev Setup

1. Install Python, dev & mysql tools

        sudo apt-get install pipenv python-dev libmysqlclient-dev

1. Install MySQL

        sudo apt-get install mysql-server

  1. Setup Database (be sure to change the password below)

          create database djangoapi;
          CREATE USER 'apiuser'@'localhost' IDENTIFIED BY '<<YOUR_PASSWORD>>';
          GRANT ALL PRIVILEGES ON djangoapi.* to 'apiuser'@'localhost';
          FLUSH PRIVILEGES;

1. Rename `/.env.sample` to `.env` and edit as necessary.
1. Install required packages

        pip install -r requirements.txt

1. Run migration

        python manage.py migrate
