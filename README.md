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

### Start django server
```python
    python manage.py runserver
```

### Run migration and create db.sqlite3
```python
    python manage.py makemigration
    python manage.py migrate
```

### Create Super user for django admin
```python
    python manage.py createsuperuser
```

### Create a new component for model/web-application
```python
    python manage.py startapp <appname>/<component_name>
```

### Run python shell
```python
    python manage.py shell
```

### Importing/accessing global variables defined in settings.py
```python
    from django.conf import settings
```

### Retreive global data stored in variable GLOBAL_VAR
```python
    from django.conf import settings
    GLOBAL_VAR_NEW = getattr(settings, 'GLOBAL_VAR', 'default')
```

### Standard way to import modules/models
```python
    from <appname>.models import <CLASSNAME>
```

### Get a single stored item
```python
    EmailEntry.objects.get(id=1)
    EmailEntry.objects.get(email="vasudeveloper001@gmail.com")
```

### Listing all stored items of a Model
```python
    EmailEntry.objects.all()
```

### Filter all stored items of a model
```python
    EmailEntry.objects.filter(email="vasudeveloper001@gmail.com")    
```

### Create a new stored item (instance) of a Model
```python
    EmailEntry.objects.create(email="saurabh3131995@gmail.com")
```
or
```python
    obj = EmailEntry()
    obj.email = "vasudeveloper001@gmail.com"
    obj.save()
```

### Update a new stored item (instance) of a Model
```python
    obj = EmailEntry.objects.get(id=1)
    obj.name = "Vasu Srivastava"
    obj.save()
```

### Delete a stored item
```python
    obj = EmailEntry.objects.get(id=3)
    obj.delete()
```

## Source

CodingEntrepreneurs: https://www.youtube.com/watch?v=bY-zab0JWWk