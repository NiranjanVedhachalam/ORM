# Ex02 Django ORM Web Application
## Date: 16-04-2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![ChatGPT Image Apr 16, 2025, 08_31_35 AM](https://github.com/user-attachments/assets/2d87bc77-5d30-410c-81fa-4ab086c8e92d)


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

```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    USER_ID=models.IntegerField(primary_key=True)
    USER_NAME=models.CharField(max_length=100)
    PHONE_NUMBER=models.IntegerField()
    EMAIL=models.EmailField()
    MOVIE_NAME=models.CharField(max_length=100)
    SEATS=models.IntegerField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('USER_ID','USER_NAME','PHONE_NUMBER','EMAIL','MOVIE_NAME','SEATS')


```

## OUTPUT

![web exp2 ](https://github.com/user-attachments/assets/c0adf187-d20c-4dbe-89e3-528826a4832e)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
