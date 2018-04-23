# Notes and resources for installation/setup of Python/Django

_This is a work-in-progress, and may be adjusted or moved/incorporated with
other material._

## Getting started
Start by making sure you have Python 3 and pip installed. You may already, and
can check at the command line:

```
python --version  # Should be >3
pip --version     # Should be >9
```

If you don't, then installation depends on your platform - for MacOS (which has
Python 2 by default), `brew install python` gives Python 3. For Linux, similar
commands should work for your native package manager. For Windows, you can
use: https://www.python.org/downloads/

## Key concepts to know

- Python development uses virtual environments to encapsulate both the
dependencies and the actual binaries for the version of Python/pip being used.
The common paradigm is to create a virtual environment to use with a project,
and then activate that environment in the shell before starting work.
- Git is an important part of our development flow, and you will want to start
getting comfortable with branches, merging, and other more "powerful" use cases.
- SQLite is great for local development, but for deploying we will be using
PostgreSQL or similar. Your project can be configured to switch/use both.
- Do not check in secrets or your virtual environment! Official repos have a
`.gitignore` to help prevent this, and if you create your own repos the
GitHub-provided `.gitignore` if you select Python as the language for your repo
is pretty good.

## Common commands to know

- Python
  - `pip install -r requirements.txt` - install Python packages from a requirements.txt file
  - `virtualenv env` - create a new virtual environment in the directory `./env`
  - `source bin/activate` - activate virtual environment created by `virtualenv`
  - `pipenv install` - newer command, both installs dependencies *and* makes an environment
  - `pipenv shell` - activate virtual environment created by `pipenv`
- Django
  - `python manage.py runserver` - start the Django server
  - `python manage.py makemigrations` - create migrations (SQL update statements) based on model changes
  - `python manage.py migrate` - apply migrations to the database
  - `python manage.py help` - see available commands and get help for them
- Heroku
  - `heroku login` - authorize the Heroku CLI with your account
  - `heroku create your-app` - make a new Heroku application (execute within your repository)
  - `heroku addons:create heroku-postgresql:hobby-dev` - make a PostgreSQL db and configure the `DATABASE_URL` environment variable so Django can connect to it
  - `git push heroku master` - deploy to Heroku
- Git
  - `git fetch upstream` - pull down upstream changes to your local repository
  - `git branch` - see a list of what branches are available
  - `git checkout -b newbranch` - make a new branch (usually do this before committing new changes)
  - `git checkout otherbranch` - switch to another (existing) branch
  - `git merge otherbranch` - merge another branch into your current branch

## Resources
You do not need to use *all* of these, but check them out and see which ones
work well for you.

- Python
  - http://docs.python-guide.org/en/latest/intro/learning/
  - https://docs.python.org/3/
  - https://github.com/arogozhnikov/python3_with_pleasure
  - https://repl.it/languages/Python3
  - https://marketplace.visualstudio.com/items?itemName=ms-python.python
  - https://code.visualstudio.com/docs/python/environments
  - https://docs.python.org/3.6/library/pdb.html
  - https://docs.pipenv.org/
  - https://github.com/pypa/pipfile
- Django
  - https://docs.djangoproject.com/en/2.0/intro/
  - https://djangopackages.org/
  - http://awesome-django.com/
  - https://spapas.github.io/2017/10/11/essential-django-packages/
  - https://djangobook.com/the-django-book/
  - https://tutorial.djangogirls.org/en/
  - https://simpleisbetterthancomplex.com/
  - https://www.fullstackpython.com/django.html
  - https://www.codingforentrepreneurs.com/blog/install-python-django-on-windows/
  - https://www.codingforentrepreneurs.com/blog/install-django-on-mac-or-linux/
  - https://dev.to/grahamlyons/the-quickest-way-to-run-python-in-docker-165
  - https://github.com/graphql-python/graphene-django
  - https://gearheart.io/blog/using-graphql-with-django/
  - https://github.com/pennersr/django-allauth
  - http://www.django-rest-framework.org/
  - https://hackernoon.com/creating-websites-using-react-and-django-rest-framework-b14c066087c7
  - https://stackoverflow.com/questions/41867055/how-to-get-django-and-reactjs-to-work-together
  - https://blog.doordash.com/tips-for-building-high-quality-django-apps-at-scale-a5a25917b2b5
  - http://www.paulox.net/2017/12/22/full-text-search-in-django-with-postgresql/
- Heroku
  - https://devcenter.heroku.com/articles/heroku-cli
  - https://devcenter.heroku.com/articles/getting-started-with-python#introduction
  - https://devcenter.heroku.com/articles/config-vars
  - https://medium.com/@nicholaskajoh/deploy-your-react-django-app-on-heroku-335af9dab8a3
- Git
  - https://www.atlassian.com/git/articles/git-forks-and-upstreams
  - https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
  - https://hackernoon.com/lesser-known-git-commands-151a1918a60
- Other
  - https://www.howtographql.com/
  - https://www.postgresql.org/docs/
  - https://sqlite.org/cli.html
  - http://latacora.singles/2018/04/03/cryptographic-right-answers.html
