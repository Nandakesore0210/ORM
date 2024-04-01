# Ex02 Django ORM Web Application
## Date: 1/4/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![screenshot 2](https://github.com/Nandakesore0210/ORM/assets/149365088/6c141bf1-8502-4353-80b2-c5c7ad8e90fe)

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
    list_display=("title","author_name","book_id","number_of_pages","year_of_publishing","book_price",);

admin.py

from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
```

## OUTPUT

![Screenshot (1)](https://github.com/Nandakesore0210/ORM/assets/149365088/e8427ec4-6068-412f-b79b-3d2b6697876b)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
