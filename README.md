Process Boy
===========

A process manager inspired by Procfile-based Foreman.
Aims to make it a breeze to run multiple processes on the background
for development.

Requires Python 3.4+

Running
=======
A `Procfile` contains a list of processes to run.

```
django: python manage.py runserver
redis: redis-server --port 6380
```

An optional `.env` file contains environment variables available for the
running processes.

```
DJANGO_SETTINGS_MODULE=project.settings
```

Then, run it all.

```
$ procboy
```

Similar
=======

- [honcho](https://honcho.readthedocs.org/en/latest/)
