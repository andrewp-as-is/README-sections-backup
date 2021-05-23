```bash
$ export DJANGO_SETTINGS_MODULE='django_migrations_settings'
$ django-admin.py makemigrations
```

custom `INSTALLED_APPS`
```bash
$ export DJANGO_SETTINGS_MODULE='django_migrations_settings'
$ export DJANGO_INSTALLED_APPS='app1,app2,app3'
$ django-admin.py makemigrations
```
