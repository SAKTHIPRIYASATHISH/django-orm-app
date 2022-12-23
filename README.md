# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1: 
create a django project

### STEP 2:
create a superuser

### STEP 3:
make migrations


## PROGRAM
### in admin.py:
```
from django.contrib import admin
from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)
```

### in models.py :
```
from django.db import models
from django.contrib import admin

class Student (models.Model):
    referencenumber = models.CharField (max_length=10,primary_key=True)
    name = models.CharField(max_length=100)
    age = models.IntegerField()
    email = models.EmailField()
    dateofbirth = models.DateField()

class StudentAdmin(admin.ModelAdmin):
    list_display = ('referencenumber','name','age','email','dateofbirth')
```

## OUTPUT

Include the screenshot of your admin page.


## RESULT
Developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
