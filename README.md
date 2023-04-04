# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ENTITY RELATIONSHIP DIAGRAM](./output2.png)
## DESIGN STEPS

### STEP 1:
clone the problem form github 

### STEP 2:
create new app

### STEP 3:
Enter the code for admin.py and model.py

### STEP 4:
Execute Django admin and create 10 students 

Write your own steps

## PROGRAM

I```
Model.py

from django.db import models
from django.contrib import admin
class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')

Admin.py

from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)

```

## OUTPUT

![OUTPUT](./output.png)


## RESULT
program executed successfully