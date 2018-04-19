# README

Just a testing place for learning Django REST API & Azure AD

## Dev Setup

1. Install Python, dev & mysql tools
  - `sudo apt-get install pipenv python-dev libmysqlclient-dev`
1. Install mysql `sudo apt-get install mysql-server`
  1. Create Database called djangoapi `create database djangoapi;`
  1. Create user `CREATE USER 'apiuser'@'localhost' IDENTIFIED BY 'P@ssw0rd123';`
1. Grant permissions `GRANT ALL PRIVILEGES ON djangoapi.* to 'apiuser'@'localhost';`
1. Rename `mysql.cnf.sample` to `mysql.cnf` and edit as necissary.
1. Install required packages `pip install -r requirements.txt`
1. Run migration `python manage.py migrate`