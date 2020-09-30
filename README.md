# DARKWEB

This used to be the repository holding the DarkScience website, that has been
moved to https://git.drk.sc/darkscience/darkscience.net.

At the moment this repository contains a Django application which powers the
quotes system for DarkScience. This is a legacy part of the old website still
in service.

## DEVELOPMENT ENVIRONMENT

You can configure a development environment with the following:

**NOTE**: *These steps assume you have Python along with pipenv installed.*

```bash
$ pipenv install --dev
# configure URL to DB (can be sqlite locally)
$ export DATABASE_URL="sqlite:///$(pwd)/db.sqlite"
$ pipenv run python manage.py migrate
```

### RUNNING THE TESTS

```bash
$ pipenv run python manage.py test
```

### RUNNING THE DEVELOPER SERVER

```bash
$ pipenv run python manage.py runserver
```

