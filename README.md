# Ex02 Django ORM Web Application
## Date: 6-12-2025
## Ref no:25013558

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM



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
~~~
models.py

from django.db import models 
from django.contrib import admin
class amazon_DB (models.Model):
     Product_name=models.CharField(max_length=20)
     S_no=models.IntegerField (primary_key=True)
     Product_type=models.CharField(max_length=20)
     Price=models.CharField(max_length=20)
     Year=models.IntegerField()
class amazon_DBAdmin(admin.ModelAdmin):
     list_display=["Product_name","S_no","Product_type","Price","Year"]

admin.py

from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)
~~~




## OUTPUT
<img width="1919" height="1079" alt="Screenshot 2025-12-06 110053" src="https://github.com/user-attachments/assets/56025262-6e4d-435c-b683-9b07c94363fe" />

<img width="1919" height="1076" alt="Screenshot 2025-12-06 110027" src="https://github.com/user-attachments/assets/1f9655c3-f4ef-49af-8f89-8fa446a18345" />


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
