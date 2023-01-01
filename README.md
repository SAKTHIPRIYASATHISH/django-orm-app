# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![er1](https://user-images.githubusercontent.com/119104282/210168195-cfa9e71f-4596-4cd1-9ef5-a5587f422801.jpg)


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
![terminal](https://user-images.githubusercontent.com/119104282/210139708-5460a115-592d-4462-b7e1-9528c46a10bf.png)
![out](https://user-images.githubusercontent.com/119104282/210139795-fe7dfbc7-38a0-434d-8d07-099a1405bfd3.jpg)





## RESULT
Developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
