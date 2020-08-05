# hello_django2
Second Hello Django

It's time for some hands-on experience building your first Django project!

Django's official website (Links to an external site.)Links to an external site. has the following to say about the web framework: "Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of Web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source."

Sounds like a pretty sweet deal! Learning to use Django will allow us to build what we want, without encountering many of the web development woes that come with building something from scratch or employing a microframework (Links to an external site.)Links to an external site., e.g., Express.js or Flask. 

To get a feel (Links to an external site.)Links to an external site. for what it's like to build a Django web application, let's focus on creating a simple project.

Your Task
Build a Django web application that displays "hello, world" (Links to an external site.)Links to an external site..

To do this, you'll need the following:

a Django project named `hello_django`
a Django app named `hello_app`
a `urls.py` file in `hello_django`
`urls.py`
sets up an endpoint for the root of the application, i.e., http://127.0.0.1:8000/ (Links to an external site.)Links to an external site.
you'll want to hook this endpoint up with a view
sets up an endpoint/path for the admin panel
this should already be a part of your `urlpatterns` if you used `django-admin` to create your project
a `views.py` file in `hello_app`
`views.py` will contain a view called `index_view`
`index_view` will render the `index.html` template with context passed to the template i.e. "hello, world"
a folder named `templates`
this folder should live at the same level as your `hello_django` and `hello_app` folders
a file in your `templates`directory called `index.html`
this file will display the "hello, world" text
"hello, world" cannot be hardcoded into this file; it must come from the view.
a `settings.py` that is properly configured
Django needs to know where to find the template folder
configure the `TEMPLATES` variable in `settings.py`
Django needs to know about the `hello_app` we're using
configure the `INSTALLED_APPS` variable in `settings.py`
a `pyproject.toml` file with Django listed as a dependency
File Structure Preview: 
.
├── hello_app
│   ├── __init__.py
│   ├── urls.py
│   └── views.py
├── hello_django
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py
├── poetry.lock
├── pyproject.toml
└── templates
    └── index.html


Submission
Create a new GitHub (Links to an external site.)Links to an external site. repo
Push your code up to the master branch of the new GitHub repo
Submit a link to the repo
https://github.com/<github_username>/hello_django


Rubric
Oh, hi Django!
Oh, hi Django!
Criteria	Ratings	Pts
This criterion is linked to a Learning Outcomehttp://127.0.0.1:8000/ displays a page with "hello, world"
1.0 pts
Full Marks
shows up on the index page & passed in through the view
0.5 pts
hardcoded into the template, not passed in through the view
0.0 pts
No Marks
"hello, world" is not displayed at all
1.0 pts
This criterion is linked to a Learning Outcomeurls.py is set-up correctly
1.0 pts
Full Marks
`hello_django/urls.py` is setup to serve the `index_view` at http://127.0.0.1:8000/
0.5 pts
Some of the way there, but there are issues
0.0 pts
No Marks
No attempt made to set up urls.py
1.0 pts
This criterion is linked to a Learning Outcomeviews.py set up correctly
1.0 pts
Full Marks
`index_view` is set up correctly to render `index.html` with "hello, world" passed into the context dictionary
0.5 pts
view is mostly there, but there are problems
0.0 pts
No Marks
view not set up correcly
1.0 pts
This criterion is linked to a Learning Outcomesettings.py set up correctly
1.0 pts
Full Marks
Both TEMPLATES and INSTALLED_APPS is set up correctly
0.5 pts
TEMPLATES or INSTALLED_APPS is set up correctly, but there are issues
0.0 pts
No Marks
neither TEMPLATES nor INSTALLED_APPS is configured correctly
1.0 pts
This criterion is linked to a Learning OutcomeRepo contains pyproject.toml that includes all necessary dependencies to run application
1.0 pts
Full Marks
running poetry install succeeds in creating a virtual environment and installing django
0.5 pts
poetry install just creates a virtual environment, but does not install django
0.0 pts
No Marks
poetry install fails due to a misconfigured pyproject.toml
1.0 pts
Total Points: 5.0