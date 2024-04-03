# Ex02 Django ORM Web Application
## Date: 
03/04/24
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/lakshman1206/ORM/assets/129931784/22b87344-0733-444c-a3e8-3f6374880803)


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
     bookid=models.IntegerField(primary_
     key=True);
     bookname=models.CharField(max_length=20);
     author=models.CharField(max_length=50);
     price=models.IntegerField();
     publishdate=models.DateField();
class BookAdmin(admin.ModelAdmin):
     list_display=("bookid","bookname","author","price","publishdate");

admin.py
from django.contrib import admin
from .models import Book ,BookAdmin
admin.site.register(Book,BookAdmin)
```

## OUTPUT

![image](https://github.com/lakshman1206/ORM/assets/129931784/e4d6a8fa-2440-4a48-ae95-ecdf60c911b9)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
