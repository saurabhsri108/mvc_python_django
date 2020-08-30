# Python MVC Django 3.1 Start Project

This is a simple learning project as an intro to Python Django 3.1 MVC Pattern landing page.

## Important Notes

1. DATABASES is defined in settings.py file.
2. migrate command must be run before createsuperuser command.
3. startapp is a command use to build a new component like module.
4. models.py is where data table model is define using classes in python extending django Model class inside models module
5. admin.py is where we register our newly created models.
6. Once model is registered, django admin will show it on its panel

## Commands

    1. python manage.py runserver # to start django server
    2. python manage.py migrate # to run migration and create db.sqlite3 file
    3. python manage.py createsuperuser # to create super user for django admin
    4. python manage.py startapp __appname__ # to create a new component for web application
    

## Source

CodingEntrepreneurs: https://www.youtube.com/watch?v=bY-zab0JWWk