# django tutorial

## After you pull
Please use virtualenv.
Create virtual environment and activate:
```
virtualenv env
source env/bin/activate
```
Then install packages using requirements file:
```
pip install -r requirements.txt
```

## Before you commit and push
Before you commit:
```
pip freeze > requirements.txt
```

## database requirements
Make sure docker and docker-compose is installed for the following.
To start the db:
```
docker-compose up -d
```

For mysql the following will help solve issues of `migrate`:
https://pypi.org/project/mysqlclient/
https://stackoverflow.com/questions/46902357/error-loading-mysqldb-module-did-you-install-mysqlclient-or-mysql-python
https://stackoverflow.com/questions/55657752/django-installing-mysqlclient-error-mysqlclient-1-3-13-or-newer-is-required
