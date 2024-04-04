# Ex02 Django ORM Web Application
## Date: 04.04.2024

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
~~~

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

~~~

## OUTPUT

![Screenshot 2024-04-04 183806](https://github.com/dhanamoni/ORM/assets/151629757/dba1db94-8f5a-4fb5-b326-72fca75db1a8)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
