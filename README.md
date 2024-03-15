# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

admin.py

from django.contrib import admin
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)

models.py

from django.db import models
from django.contrib import admin
class footballplayer (models.Model):
    name=models.CharField(max_length=15)
    weight=models.IntegerField()
    age=models.IntegerField()
    members=models.CharField(max_length=20)
    experiance=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('name','weight','age','members','experiance')




## OUTPUT

![image](https://github.com/Dilliarasu0105/ORM/assets/144979593/8a5d56c5-f6ba-4bd8-908d-1b378aab5827)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
