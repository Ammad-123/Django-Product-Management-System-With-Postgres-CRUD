1 - Create a Django Project and App

django-admin startproject myproject
cd myproject
python manage.py startapp myapp

2 - Configure PostgreSQL Database
Update the DATABASES setting in myproject/settings.py:
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'yourdbname',
        'USER': 'yourdbuser',
        'PASSWORD': 'yourdbpassword',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}



------ Apply migrations
python manage.py makemigrations
python manage.py migrate


----- Run Project
python manage.py runserver
