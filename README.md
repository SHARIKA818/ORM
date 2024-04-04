# Ex02 Django ORM Web Application
## Date: 03/04/2024

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
```
models.py
from django.db import models
from django.contrib import admin
class Book(models.Model):
title=models.CharField(max_length=20);
author_name=models.CharField(max_length=30);
author_name=models.CharField(max_length=30);
book_id=models.IntegerField();
number_of_pages=models.IntegerField();
year_of_publishing=models.DateField();
book_price=models.IntegerField();
class BookAdmin(admin.ModelAdmin):
list_display=("title","author_name","book_id","number_of_pages","year_of_publishing","book_p
admin.py
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
```
## OUTPUT

![967cad59-fa92-4f1b-abe6-aeedb1fe15f6](https://github.com/SHARIKA818/ORM/assets/139834761/0393c2d8-fba2-4e1b-8c8f-3c686f8059ca)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
