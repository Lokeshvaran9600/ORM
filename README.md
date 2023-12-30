# Ex02 Django ORM Web Application
## Date: 29.12.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
admin.py
from django.contrib import admin
from.models import foodball_player,foodball_playerAdmin
admin.site.register(foodball_player,foodball_playerAdmin)

models.py
from django.db import models
from django.contrib import admin 
class foodball_player(models.Model):
    p_name=models.CharField(max_length=20)
    p_age=models.IntegerField()
    p_country=models.CharField(max_length=20)
    p_email=models.EmailField()
    p_salary=models.IntegerField()

class foodball_playerAdmin(admin.ModelAdmin):
    list_display=('p_name','p_age','p_country','p_email','p_salary')
```



## OUTPUT
![WhatsApp Image 2023-12-30 at 07 06 51_788e6627](https://github.com/Lokeshvaran9600/ORM/assets/145972263/2a8be4d8-6415-4443-9672-0298a4bdedc9)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
