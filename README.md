# Ex02 Django ORM Web Application
## Date: 18-09-2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM


![Screenshot 2024-09-18 090214](https://github.com/user-attachments/assets/52387c80-0a56-4124-9e5f-6b2192eebf39)



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
from.models import Bankloan,Bankloanadmin
admin.site.register(Bankloan,Bankloanadmin)

model.py    
    from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
    Loanid=models.IntegerField(primary_key=True)
    Customername=models.CharField(max_length=50)
    Salary_slips=models.IntegerField()
    Accountno=models.IntegerField()
    Adharno=models.IntegerField()
    
    
class Bankloanadmin(admin.ModelAdmin):
    list_display=('Loanid','Customername','Salary_slips','Accountno','Adharno')
```


## OUTPUT

Include the screenshot of your admin page.

![Screenshot 2024-09-18 090207](https://github.com/user-attachments/assets/056aad86-1047-4fda-ac15-989ef952c6eb)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
