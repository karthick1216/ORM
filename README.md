# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![alt text](<er diagram.jpg>)
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
admins.py

from django.contrib import admin
from.models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)


models.py

from django.db import models
from django.contrib import admin
class Loan(models.Model):
   lid=models.CharField(max_length=15,primary_key="lid")
   loantype=models.CharField(max_length=15)
   name=models.CharField(max_length=15)
   age=models.IntegerField()
   aadhar=models.IntegerField()
   documents=models.CharField(max_length=15)

class LoanAdmin(admin.ModelAdmin):
    list_display=('lid','loantype','name','age','aadhar','documents')
# OUTPUT
![alt text](<Screenshot 2024-11-20 162048.png>)
![alt text](<Screenshot 2024-11-20 162627.png>)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
