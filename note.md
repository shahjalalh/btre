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

## 06: Models, Migrations & Admin

https://postgresapp.com/ for Mac PostgreSQL installer

To set the password in new PostgreSQL installation, go to postgresql console -
```
postgres=# \password postgres
Enter new password: 
postgres=# 
postgres=# CREATE DATAGASE btredb OWNER postgres;
postgres=# 
postgres=# \l
postgres=# 
postgres=# \q
```

Install pgadmin 4 in mac

Install Postgres dependencies in django project. In the virtual environment - 
```
$ pip install psycopg2 psycopg2-binary
```

update /btre/settings.py for PostgreSQL db DATABASES = {} 

run migration - 
```
$ python manage.py migrate

```
Django fields reference:

https://docs.djangoproject.com/en/2.2/ref/models/fields/


update listings/models.py Listing model <-----------

update realtors/models.py Realtor model

migrate
```
$ python manage.py makemigrations
$ pip install Pillow
$ python manage.py makemigrations
$ python manage.py migrate
```

creating superuser
```
$ python manage.py help
$ python manage.py createsuperuser
```

> **Staff status** - user can login to admin area or not

update listings/admin.py

update btre/btre/settings.py MEDIA_URL and MEDIA_ROOT

update btre/btre/urls.py with + static(settings.MEDIA_URL, ....)

populate data in realtors and listings from html template.

create and update /templates/admin/base_site.html

create and update /btre/btre/static/css/admin.css  

update /listings/admin.py for admin custom list view (ListingAdmin)

update /realtors/admin.py for admin custom list view (RealtorAdmin)

06: class done and practical not done
