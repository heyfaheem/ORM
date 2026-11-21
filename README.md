# Ex02 Django ORM Web Application
## Date: 21-11-2026
FAHEEM AHMED S

## AIM
To develop a Django Application to store and retrieve data from a Vehicle Service Database platform using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM
```
models.py

from django.db import models
from django.contrib import admin

class user(models.Model):
    Gmail=models.EmailField()
    Mobile_No=models.IntegerField()
    Username=models.CharField(max_length=10,primary_key=True)
    Address=models.TextField()
    Product_Type=models.CharField(max_length=15)
    Product_Name=models.CharField(max_length=15)
    Apply_Coupon=models.CharField(max_length=10)
    
class userinfo(admin.ModelAdmin):
    list_display=["Gmail","Mobile_No","Username","Address","Product_Type","Product_Name","Apply_Coupon"]


admin.py
from django.contrib import admin
from .models import user,userinfo
admin.site.register(user,userinfo)

```



## OUTPUT
<img width="619" height="343" alt="image" src="https://github.com/user-attachments/assets/62e9df8d-e5bc-4143-b4a4-ee13570a6d97" />




## RESULT
Thus the program for creating vehicle service Database using ORM hss been executed successfully.
