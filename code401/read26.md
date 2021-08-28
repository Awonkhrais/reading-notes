# Intro to Django

![](https://www.letsrundigital.com/blog/wp-content/uploads/2017/12/LRD-Blog-1-810x423.png)

**Django is a Python-based web framework used by millions of developers and billions of consumers through popular apps like Instagram.**

**It is open source, meaning the code is available for free on Github and can be downloaded onto any developer’s computer and used alongside the official documentation.**

## Django Model-View-Controller Pattern (MVC):

![MVC](https://www.tutorialandexample.com/wp-content/uploads/2020/01/Controller-in-Django.png)

## Starting project with Django :

Creating a project:

```django-admin startproject mysite```

The development server:

```python manage.py runserver```

Creating the Polls app:

```python manage.py startapp polls```

Write your first view:

Let’s write the first view. Open the file polls/views.py and put the following Python code in it:

```py
from django.http import HttpResponse


def index(request):
    return HttpResponse("Hello, world. You're at the polls index.")

```

In the polls/urls.py file include the following code:

```py

from django.contrib import admin
from django.urls import include, path

urlpatterns = [
    path('polls/', include('polls.urls')),
    path('admin/', admin.site.urls),
]
```