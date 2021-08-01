# Django-Project-Environment-setup-with-Virtual-Environment

# Create the project directory
-> mkdir project_folder
-> cd project_folder

# Install the virtualenv package
-> pip install virtualenv

# Create a virtual environment
-> virtualenv env_name

# Activate the virtual environment
-> On Windows use .\env_name\Scripts\activate 
-> On mac source env/bin/activate

# Install Django 
-> pip install django

# Set up a new project with a single application
-> django-admin startproject projectName .  # Note the trailing '.' character
-> cd projectName
-> django-admin startapp appName
-> python manage.py startapp appName
-> python manage.py makemigrations
-> python manage.py migrate
-> python manage.py createsuperuser
-> python manage.py runserver

# set 


# Add 'appName' to INSTALLED_APPS. The settings module will be in projectName/settings.py
INSTALLED_APPS = [
    ...
    'appName',
]


# Add Bangladeshi time zoon 'Asia/Dhaka' to TIME_ZONE. The settings module will be in projectName/settings.py
TIME_ZONE = 'Asia/Dhaka'


# Install Django REST framework into the virtual environment
pip install djangorestframework

# Add 'rest_framework' to INSTALLED_APPS. The settings module will be in projectName/settings.py

INSTALLED_APPS = [
    ...
    'rest_framework',
]
