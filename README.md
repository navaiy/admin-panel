This admin panel has been edited by jazzmin and works only for the rtl languages

![sds](jazzmin/static/a3.png)
![sds](jazzmin/static/a1.png)
![sds](jazzmin/static/a2.png)


## Installation
```
pip install django-admin-panel-arnika

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
from django.urls import include
from jazzmin.view import register

urlpatterns = [
    path("i18n/", include("django.conf.urls.i18n")),
    path("", include("django.contrib.auth.urls")),
    path('register', register, name='register'), ]
]
```
