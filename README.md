Process Boy
===========

A process manager to help run development enviroments with ease.

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

For custom environment and processes, use local files:

```
$ procboy -e .env.dev -f Procfile.dev
```
