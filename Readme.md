python -m venv env

env/Scripts/activate

pip install django

pip install djangorestframework

django-admin help

django-admin startproject Backend

cd Backend

python manage.py startapp api

rest_framework - update in the Backend settings.py

python manage.py migrate

python manage.py createsuperuser

python manage.py runserver

http://localhost:8000/


user: yogesh
pass: may@2024

**Setting up Authentication**

pip install djangorestframework_simplejwt 

add this in the setting.py 


REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.AllowAny',
    ],
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
        # Add other authentication classes if needed
    ],
}

**Create a Requirements.txt file**

pip freeze > requirements.txt

**Create Docker File**

write the commands and create the docker File 

