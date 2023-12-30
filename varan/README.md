# Ex04 Places Around Me
## Date: 29.12.2023

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
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
![Alt text](<WhatsApp Image 2023-12-30 at 07.06.51_587e286e.jpg>)


## RESULT
The program for implementing image maps using HTML is executed successfully.
