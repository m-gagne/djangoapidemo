# README

Just a testing place for learning Django REST API & Azure AD

## Dev Setup

1. Install Python

        sudo apt-get install pipenv

1. Install MySQL

        sudo apt-get install mysql-server

    - *Note* if you are running this under WSL (bash on Windows) you will need to manually start the sql service by running `sudo service mysql start`

1. Setup Database

    - Connect to mysql server `mysql -u root -p` and run the following SQL below, be sure to change the password in the CREATE USER statement.

          create database djangoapi;
          CREATE USER 'apiuser'@'localhost' IDENTIFIED BY '<<YOUR_PASSWORD>>';
          GRANT ALL PRIVILEGES ON djangoapi.* to 'apiuser'@'localhost';
          FLUSH PRIVILEGES;

1. Rename `/.env.sample` to `.env` and edit as necessary.
1. Install required packages

        pip install -r requirements.txt

1. Run migration

        python manage.py migrate
