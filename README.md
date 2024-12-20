 Ex02 Django ORM Web Application
# Date:30/09/24
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-12-07 220352](https://github.com/user-attachments/assets/7e2493ca-a1f4-485d-81e4-c98996f4e574)

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
models.py
from django.db import models
from django.contrib import admin
class Bankloan(models.Model):
name=models.CharField(max_length=100)
accno=models.IntegerField(primary_key="accno")
ifscno=models.IntegerField()
mobno=models.IntegerField()
email=models.EmailField()
class BankloanAdmin(admin.ModelAdmin):
list_display=('name','accno','ifscno','mobno','email')
admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)

```
# OUTPUT
![Screenshot 2024-12-07 220439](https://github.com/user-attachments/assets/56d025a4-e0f7-4753-89c3-82a0e8a11b57)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
