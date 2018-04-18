# README   

Just a testing place for learning Django REST API & Azure AD

## Dev Setup

1. Install Python & Django
1. Install mysql `sudo apt-get install mysql-server`
1. Install mysql for python library `sudo apt-get install python-mysqldb`
1. Rename `mysql.cnf.sample` to `mysql.cnf` and edit as necissary.
1. Install `MySQL`
1. Create Database called djangoapi `create database djangoapi;`
1. Create user `CREATE USER 'apiuser'@'localhost' IDENTIFIED BY 'P@ssw0rd123';`
2. Grant permissions `GRANT ALL PRIVILEGES ON djangoapi.* to 'apiuser'@'localhost';`