# Ex02 Django ORM Web Application
## Date: 03.03.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-04-04 192112](https://github.com/Sandhniya/ORM/assets/151395890/5ee95ee0-b536-4160-8d77-1ab25db35894)


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

DEVELOPED BY:SANDHIYA SREE.B
REG NO:212223220093
```
models.py
from django.db import models
from django.contrib import admin
class Employee(models.Model):
    eid=models.CharField(max_length=20,help_text='Employee_ID')
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

admin.py
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

```

## OUTPUT

![web output 1](https://github.com/Sandhniya/ORM/assets/151395890/8f41fca6-a318-45f2-bbf1-caeac97d22a7)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
