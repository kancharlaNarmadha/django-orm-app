# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Create a Django app Go to the app directory In models.py create two classes And save the models.py

### STEP 2:
Go to admins.py And put the two class in admins.py from the models.py And save the file

### STEP 3:
Start the Django server Then move to admin page



## PROGRAM:
MODELS.PY:
```
from django.db import models
from django.contrib import admin

class Student(models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    dept=models.CharField(max_length=5)


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','dept')
```
ADMIN.PY:
```
from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)
```

## OUTPUT:
![ex 2 web uhh](https://github.com/kancharlaNarmadha/django-orm-app/assets/119559316/b2aa98e4-a4ef-4fc0-be66-1374d88a7f0f)





## RESULT:
Thus the program have been executed successfully.
