# Python_Django_postgresql_PetAdoption


Python_Django_postgresql_PetAdoption

py --version

Python 3.7.5

python -m django --version

3.0.3

# settings.py

# sqlite3

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}

# postgresql

# CREATE DATABASE refugio

#psycopg2

pip install pyscopg2

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'refugio',
        'USER': 'postgres',
        'PASSWORD': 'sa',
        'HOST': 'localhost',
        'PORT': 5432,

    }
}


manage.py makemigrations
manage.py migrate

# Create User
python manage.py createsuperuser
# enter user/key:
admin
mykey

python manage.py runserver
http://127.0.0.1:8000/

http://127.0.0.1:8000/admin

http://127.0.0.1:8000/mascota/
