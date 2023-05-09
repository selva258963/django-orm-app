# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from github.

### STEP 2:
Create a new app.

### STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Create django app and add student details.

## PROGRAM
## models.py 

from django.db import models
from django.contrib import admin


class Student(models.Model):
    referencenumber=models.CharField(primary_key=true,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')


## Admin.py
from django.contrib import admin
from myapp.models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin

## OUTPUT


![Screenshot (19)](https://user-images.githubusercontent.com/121961701/237042790-7bfdd891-be56-4399-8f88-c2414f8b0e2f.png)
![Screenshot (20)](https://user-images.githubusercontent.com/121961701/237042801-23c12e97-b557-4cc7-9c69-46d2e1bc83c3.png)

## RESULT
program exiguted succesfully

