# learning-log-Django
- This is a web app called Learning Log.
- This will allow users to log in topics they are interested in and make journal  entries as they learn about the toppics.
- The Learning Log home page will describe the site and invite users to either
  register or log in.
- Once logged in, a user can create new topics, make new entries and read and
  edit existing entries.

# Creating a project
- mkdir <name of directory>
- python -m venv ll_env
- Activate virtual env: source ll_env/bin/activate
- pip install --upgrade pip
- pip install django
- django-admin startproject ll_project . Don't forget the dot at the end, this dot creates a    directory structure that will make it easy to deploy the app to a server.
-- the manage.py is a short program that takes in commands and feeds them to the relevant       parts of django

# Creating a database
- python manage.py migrate
- python manage.py runserver

# Defining Models
# Activating models
- Whenever we modify data that the Learning Log manages we follow these 3 steps:
    -- modify model.py
    -- call makemigrations on learning_logs
    -- Tell Django to migrate the project
# Migrating the Entry Model
- Migrate the database as earlier by calling makemigrations on learning_logs
    -- python manage.py makemigrations learning_logs
- and run:
    -- python manage.py migrate
