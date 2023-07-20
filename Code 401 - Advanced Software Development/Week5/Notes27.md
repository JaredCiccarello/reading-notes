July 18, 2023

Everyday there is a new django website from scratch.

Your checklist is MUCHO importante.

Why are we building things from scratch? Muscle memory.


Django is a great way to build a quick website.
___________________________________________________________
Code challenge review:
Blogs are a great way to go step by step with every change happening in your code.

Visual is theoretical. Walkthrough is practical.

You can get HELP working through something but, don't let AI take the work out of breaking something down. It will help you in the long run.

Again, AI is a geat tool but it will become a crutch in the long run. Don't let it get in the way of your learning.
___________________________________________________________



THIS IS THE STEPS FOR SETTING UP A DJANGO WEBSITE


    Lab steps: Remember, these do not necessarily have to be done in this order.

mkdir filename
create virtual environment
pip3 install django
pip3 freeze > requirements.txt

django-admin startproject projectname .
Create application: startapp filename(things)

python3 manage.py startsnacks

inside of filename(thing-rater) touch things/urls.py

python3 manage.py migrate  Migrate builds an internal model
python3 manage.py runserver

You are only seeing this page because debug is true
Changing debug to false will give you a bad request (400)
DONUT touch debug

Go into settings and add the name of your app(things)


            SQL, not important
                  Python asks about 
                  Databases uses SQL to manage things
                  Almost all relational databases use SQL
                  Sequel query language
                  Sequel analysts can make $300k

          SELECT {star} FROM users WHERE school = "CodeFellows";

          This is an example of a sequel query

          Photo located in: DJANGO folder

          We don't teach SQL because of how difficult it can be.

In urls.py
from django.db import models
from django.db 
  class Things(models.Model):
    name = models.CharField(max_length=128)
    rating = models.IntegerField(default=0)
    reviewer = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)

We create a database table
We have a name column
A rating column
This would be our MODEL

'Things' does not live inside the data



NEXT steps
  This prepares the class of Thing that you are trying to build.
python3 manage.py makemigrations Things (This is like doing git add)
python3 manage.py migrate (This is like doing a git commit)

You'll see a message applying your application of filename with an ok message.



Going to the user/admin page on your website
python3 manage.py createsuperuser
This will give you a list of inputs
Emails:
Password:

This will create the user.

Inside admin.py
from Django.contrib import admin
from .models import Thing
admin.site.register(Thing)

This will give us access to Things

In models.py
from djang.db import models
  class Things(models.Model):
    name = models.CharField(max_length=128)
    rating = models.IntergerField(default=0)
    reviewer = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)

def __str__(self):
  return self.name


Summary: Created project, created application, added application in project, created model, ran makemigration and migration, created superuser, gave permission for Django to register Things into our site.

Key difference: The site we are on is not meant for users. 
We still need to make the model viewable and give users the ability to edit.

In order to do this we will create a custom model.

In views.py
from django.views.generic import ListView
from .models import Thing

class MovieListView(ListView):
  template_name = "thing_list.html"
  model = Thing


In urls.py (at the project level)
  import include, adding this to our other import of path

urlpatterns = [
  path('admin/', admin.site.urls),
  path('', Includes('things.urls')),
]
this tells your app when you go to a home route, fix it there.


In urls.py at the things level (application level)
  from django.urls import path
  from .views import ThingsListView

urlpatterns = [
  path('', ThingsListView.as_view(), name='thing_list')
]

NEXT: we are still missing a template

mkdir templates
inside templates 
  touch base.html
  touch thing_list.html

In base.html
{% block content %}
Very basic html template

In things_list.html
{% extends 'base.html' %}

  {% block content %}
    <h1>Thing List</h1>
    {% for Thing in object_list %}
      <p>{{ thing.name }}</p>
    {% endfor %}
{% endblock content %}

When you runserver after this, you'll get an error: TemplateDoesNotExist

The Solution for this is:
In settings.py
  Under TEMAPLATES
    DIRS: [BASE_DIR / 'templates'],

In thing-rater
  In Templates
    touch thing_detail.html
{% block content %}
  <section>
    <h2>Thing Name: {{ thing.name }}</h2>
    <p>Thing Rating: {{ thing.rating }}</p>
    <p>Thing Reviewer: {{ thing.reviewer }}</p>
  </section>
{% endblock content %}

We need to pass this into our urls
In urls.py at the Things (application level)
  in addition to other elements
path{'<int:pk>', ThingDetailView.as_view(), name='thing_detail'}

Going to the url 127.0.0.1:8000/1
This will show you what our page currently holds.

In thing_list.html
  <p><a href='{% url 'thing_detail' thing.pk %}'> ({ thing.name }) </a></p>

If we wanted to create a home button
  In base.html
    <nav>
      <ul>
        <li><a href="{% url 'thing_list' %}">Home</a></li>
      </ul>
    </nav>


TESTING TESTING TESTING

  Extend your testing to your detail page
__________________________________________________

Lab 27: Django Models

create: snacks_tracker_project
snacks app
Snack model
  NO tailwind or flowbyte
Mandatory vanilla styling. CHANGE SOMETHING.

