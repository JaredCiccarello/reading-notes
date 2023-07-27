July 19, 2023

Letter                           Value
A, E, I, O, U, L, N, R, S, T       1
D, G                               2
B, C, M, P                         3
F, H, V, W, Y                      4
K                                  5
J, X                               8
Q, Z                               10

Given a value, compute the value.

Write a function, compute the score for that word.

We are given a dictionary:
POINTS = {
    'a': 1, 'b': 3, 'c': 3, 'd': 2, 'e': 1,
    'f': 4, 'g': 2, 'h': 4, 'i': 1, 'j': 8,
    'k': 5, 'l': 1, 'm': 3, 'n': 1, 'o': 1,
    'p': 3, 'q': 10, 'r': 1, 's': 1, 't': 1,
    'u': 1, 'v': 4, 'w': 4, 'x': 8, 'y': 4,
    'z': 10
}

ATTEMPT
score = 0

def letter_count():
  for letters in word
  


# TODO:
# Done:

SOLUTION:
set initial total
loop through word
odd points value to total
return total

def score_word(word):

set initial total
score = 0

loop through word
for letter in word:

odd points value to total
total += POINTS[letter]

return total
  return score

if __name__ = '__main__':
  print(score_word('cabbage')) #14
  print(score_word('za')) #11


We can also add
  if not word:
    return 0
This checks to see if the word is empty. If true, return 0.
________________________________________________

Python Library Teaching

Code out something from Python, a library.

Show us how your library works. Recommended to show the docs.

Create a 3-5 min assignment.

Due Aug 1.
_________________________________________________

Starting a new django website

mkdir filename
cd filename
python3 -m venv .venv

django-admin startproject filename

pip3 install django

Create application
python3 manage.py startapp movie

pip3 freeze > requirements.txt

mkdir templates
inside templates: 
touch filename.html
touch base.html

at root
mkdir static
In static
touch base.css

In movie
touch urls.py

WARNING WARNING: FULL SPEED AHEAD TODAY

Can we create a superuser at this point?
No, it needs a database.
You create a database when you use the MIGRATE command.

SECRET_KEY = 'lkshdaflkjsahflk'
There is a way to set up things with a .env

In movies_project (project level)
  touch .env
this DOES NOT work out of the gate

We will need a dependency environ
pip3 install django-environ
pip3 freeze > requirements.txt

In settings.py
import environ
  # Env Stuffs
  env = environ.Env(
    PUT SECRET KEY HERE,
    DEBUG = bool, False
  )
  # Read Env
  environ.Env.read_env()
  ^^^ This reads the env file

  SECRET_KEY = env.str('SECRET_KEY')
  Reading from ENV file, reading key of secret key.

This will create an env file at the project level. You should have your secret_key and debug=true 

NEXT comment out secret key inside environ and secret key on it's own. The point of this is to test if the secret_key is working.

You always want to put debug into your environ. You want this to be put to false.

  TEST this by:
  It works! We just verified that information can be pulled from our env.

FOR SUBMISSION: Put information inside of a env.txt file.


In Models.py
  class Movie(models.Model):
    name = models.CharField(max_length=64)
    description = models.TextField(default='generic description')
    owner = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)

    def __str__(self):
      return self.name
    HERE we need to create the str, when we look in our admin site, we want information.

Next we need to register this into our admin site

In admin.py
In admin.py
  from Django.contrib import admin
  from .models import Movie

  admin.site.register(Movie)

Next run
python3 manage.py makemigrations
python3 manage.py migrate
  We see here that everything was updated successfully, even our Movie app

python3 manage.py createsuperuser
  Y
Create username/password


Next we want to start working from the website we are going to build out.

In templates
touch movie-create.html
touch movie-delete.html
touch movie-detail.html
touch movie-update.html

In base.html
<!DOCTYPE html>
  <head>
    <title>My Movies</title>
  </head>
  <body>
    <header>

    </header>
    <main>
    {% block content %}
      <h2>Someone forgot to put content</h2>
    {% endblock content %}
    </main>
    <footer>
  </body>

In movie-list.html
  {%extends 'base.html' %}

  {% block content %}
    <h1>Coming Soon</h1>
  {% endblock content %}

In views.py
  from django.views.generic import ListView
  from .models import Movie
  
  class MovieListView(ListView)
    template_name = 'movie-list.html'
    model = Movie
  
In urls.py (project level)
  from django.urls import path, include

  under urlpatterns
    path('movies'/, include('movie.urls'))
  
  What does this do? This is where you do your initial route resolve. Basically, go here. If you get anything that get movies, go here and resolve this in movie.urls.

In urls.py (app level)
  from django.urls import path
  from .views import MovieListView

  urlspatterns = [
    path('', MovieListView.as_view(), name='list_view'),
  ]
At this point, do we have anything resolving our home route? No

We want our program to resolve things in our movies.


In views.py
  from django.views.generic import ListView, DetailView, CreateView
  from .models import Movie



MISSED STEP

In movie-detail.html
  {% extends 'base.html' %}

  {% block content %}
    <h1>Movie: {{ movie.name }}</h1>
    <p>Description: {{ movie.description}}
  {% endfor %}
  {% endblock content %}


In movie-list.html
    {% extends 'base.html' %}

  {% block content %}
    {% for movie in object_list %}
      <a href='{url 'detail_view' movie.pk %}' > {movie.name} </a>
  {% endfor content %}

THIS POINT IS WHERE WE LEFT OFF YESTERDAY

THIS IS WHERE THE NEW STUFF COMES IN

In views.py
  from django.views.generic import ListView, DetialView, CreateView
  
  Create new class
  Something something something

in urls.py (app level)

  ANOTHER PATH GOES HERE

  path ('new', MovieCreateView.as_view(), name='create_view'),

In ???
  {% extends 'base.html' %}

  {% block content %}
    <h1>Create a Movie<>
    <form>
      {% csrf_token %}
      {{ form.as_p }}
      <Input type="submit" value='SAVE'>
    </form>
  {% endblock content %}

csrf prevents cross site scripting. This is Django protecting you.

form.as_p gives us built in formatting. This gives us basic formatting for our webpage. This can be manipulated in different ways.
  NEXT week: We will use crispy forms

Adding data into our form on our webpage will give us an error: improperly configured at /movies/new. Provide a url or define an absolute url on the model.

This means, the form doesn't know where to send the user after this.
Solution:
  In urls.py (app level)
    under __str__
      def get_absolute_url(self):
        return reverse('detail_vew', args=[str(self.id)])
What this does, it runs a reverse lookup and look on the detail view. It'll send the detail view the self.id


In settings under project
 TEMPLATES
add 'DIRS': [BASE_DIR / 'templates']

Last 30 minutes of video are required to help complete this project.

to run your website
python3 manage.py runserver