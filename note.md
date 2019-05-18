## 05 Apps, URLs & Templates

create new app pages
```
$ python manage.py startapp pages

```

update /btre/btre/settings.py INSTALLED_APPS = []

update /pages/apps.py

create and update /pages/urls.py

update /pages/views.py

update /btre/btre/urls.py

update /btre/btre/settings.py TEMPLATES = [] 

create folder /btre/templates/pages/

create file templates/pages/index.html

create file templates/pages/about.html

update /pages/urls.py for about page

create and update /templates/base.html

create /btre/btre/static/ folder copy the content

update /btre/btre/settings.py STATIC_ROOT

run command for collect static
```
$ python manage.py collectstatic
```

update /btre/.gitignore

05:04
