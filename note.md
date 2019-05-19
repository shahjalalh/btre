## 05: Apps, URLs & Templates

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

install "Better Jinja" vs code extension

locate the template /btre/dist/

update from /dist/index.html to /templates/base.html

create and update /templates/partials/_footer.html

create and update /templates/partials/_navbar.html

create and update /templates/partials/_topbar.html

create new apps listings and realtors
```
$ python manage.py startapp listings
$ python manage.py startapp realtors
```

create and update /templates/listings/listing.html

create and update /templates/listings/listings.html

create and update /templates/listings/search.html

create and update /templates/listings/urls.py

update /btre/urls.py and add listings urls

update /btre/btre/settings.py INSTALLED_APPS = [] for listings and realtors

update /listings/views.py

05 class done and practical done
