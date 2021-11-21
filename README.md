This admin panel has been edited by jazzmin and works only for the right languages

![sds](jazzmin/static/a3.png)
![sds](jazzmin/static/a1.png)
![sds](jazzmin/static/a2.png)


## Installation
```
pip install git+https://github.com/tangentlabs/django-oscar-paypal.git@issue
```
Add jazzmin to the first list before admin app
```
INSTALLED_APPS = [
'jazzmin',
]
```
change in settings.py
```
LANGUAGE_CODE = 'fa-ir'
```
add to urls.pu
```
urlpatterns = [
    path("i18n/", include("django.conf.urls.i18n")),
]
```
