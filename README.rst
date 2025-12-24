Django shortcuts
================

You spend too much time typing ``python manage.py``.

Usage
-----

Django shortcuts installs a ``django`` binary that proxies
Django's ``manage.py`` and ``django-admin.py`` scripts.

You can use either shortcuts or full Django command names:

::

    $ django <command or shortcut>

    # Using shortcuts
    $ django r                  # runs 'runserver'
    $ django mk                 # runs 'makemigrations'

    # Using full commands
    $ django runserver
    $ django makemigrations

    # Works from any project subdirectory
    $ cd any/project/subdirectory
    $ django <command or shortcut>

Commands that work without a project (using django-admin):

::

    $ django sp myproject       # startproject
    $ django sa myapp           # startapp
    $ django version            # show Django version

Requirements
------------

Some commands require additional packages

+ South
+ Haystack
+ Django Command Extensions


Shortcuts
---------

::

    # Django
    'c'  : 'collectstatic',
    'r'  : 'runserver',
    'sp' : 'startproject',
    'sa' : 'startapp',
    't'  : 'test',

    # Django Migrations
    'mk' : 'makemigrations',
    'm'  : 'migrate',
    'mm' : 'makemigrations',

    # Shell
    'd'  : 'dbshell',
    's'  : 'shell',

    # Auth
    'csu': 'createsuperuser',
    'cpw': 'changepassword',

    # South (deprecated)
    'sd' : 'syncdb',
    'sm' : 'schemamigration',
    'dm' : 'datamigration',

    # Haystack
    'ix' : 'update_index',
    'rix': 'rebuild_index',

    # Django Extensions
    'sk' : 'generate_secret_key',
    'rdb': 'reset_db',
    'rp' : 'runserver_plus',
    'shp': 'shell_plus',
    'url': 'show_urls',
    'gm' : 'graph_models',
    'rs' : 'runscript'

Installation
------------

::

    $ pip install django-shortcuts
