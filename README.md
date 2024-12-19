# Ex02 Django ORM Web Application
# Date:10.10.2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Untitled](https://github.com/user-attachments/assets/b002de56-5987-49f0-b295-8d51d1db5a0d)





## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)
model.py
from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
    acc=models.IntegerField(primary_key="acc")
    name=models.CharField(max_length=100)
    mobileno=models.IntegerField()
    pancode=models.IntegerField()
    aadharcode=models.IntegerField()
class BankloanAdmin(admin.ModelAdmin):
    list_display=('acc','name','mobileno','pancode','aadharcode')
```
# OUTPUT

![Screenshot 2024-11-27 224429](https://github.com/user-attachments/assets/c731c571-968e-4f6b-afdc-819c39f16b19)

![web](https://github.com/user-attachments/assets/ad75ce37-94ae-4909-b3b5-4645814593cc)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
