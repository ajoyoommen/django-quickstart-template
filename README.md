# Django Quickstart Template

This repository contains a default structure for new Django projects. The setup
includes:

* A settings module.
* Database configured for PostgreSQL with psycopg2 in requirements.
* Scripts to source a virtual environment, load constants and start dev server.
* Error logging configuration for production.

## Installation

1. Download the template for [Django 1.10.2][latest].
2. Install a virtualenv and update `env.sh`.
3. Rename folder `django_project` to your project's name.
4. Update your project's name in the following django files:

```
   * manage.py
   * settings/common.py
   * settings/dev.py
   * settings/__init__.py
   * wsgi.py
   * urls.py
 ```

5. Update `start.sh` to point to your project's dev settings.

## Configuration

Export the following (required) variables in `env.sh`:
* `SECERT_KEY`
* `DBNAME`
* `DBPASS`
* `DBUSER`
* `STATIC_ROOT`
* `MEDIA_ROOT`
* `ERROR_LOG`

## Usage

To start a dev server, run

    ./start.sh

[latest]: https://github.com/ajoyoommen/django-quickstart-template/archive/django-1.10.2.zip
