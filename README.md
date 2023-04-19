# Django ORM Web Application

## AIM 

To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![er](https://user-images.githubusercontent.com/122548204/233128484-212f1d91-0b5b-424f-96bb-0949f92261ac.png)


## DESIGN STEPS

### STEP 1: 

 Clone the problem from github

### STEP 2:
 
Create a new app

### STEP 3:

Enter the code for admin.py and model.py

### STEP 4:

Execute Django admin and create 10 employees

## PROGRAM
```
Models.py 

from django.db import models
from django.contrib import admin
class Student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    marks=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class StudentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','marks','age','email') 

Admin.py 

from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)
```
## OUTPUT
 
![admin1](https://user-images.githubusercontent.com/122548204/233128328-7009af73-3134-4e11-bc82-349c600c2afb.png)


## RESULT

Program executed successfully.
