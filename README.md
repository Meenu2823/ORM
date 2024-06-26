# Ex02 Django ORM Web Application
## Date: 02.04.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub.

### STEP 2:
Create a new app in Django project.

### STEP 3:
Enter the code for admin.py and models.py.

### STEP 4:
Execute Django admin and create details for 10 books.

## PROGRAM

~~~
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee(models.Model):
    empid=models.IntegerField()
    empname=models.CharField(max_length=20)
    dept=models.CharField(max_length=10)
    salary=models.FloatField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('empid','empname','dept','salary')
~~~

## OUTPUT

![Screenshot 2024-04-02 203634](https://github.com/Meenu2823/ORM/assets/139416219/64a025f9-4fc4-468a-bf43-56ecd73770ee)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully.
