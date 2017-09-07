https://github.com/ijinmao/BiMPM_keras
https://github.com/bradleypallen/keras-quora-question-pairs

https://github.com/adaptives/python-examples
https://github.com/geekcomputers/Python

https://github.com/gothinkster/django-realworld-example-app
https://github.com/django-ve/helloworld

https://github.com/django-ve/helloworld/blob/master/helloworld/views.py

```python
# -*- coding: utf-8 -*-
from django.http import HttpResponse

def index(request):
return HttpResponse("Hello, world!")
```

On the example code above, we can see and understand how Django basic request looks like, that code means, whenever the definition 'index' is called, the definition will return the http response, in this case it's just basic string saying "Hello, world!".

Below, we have routing example code for Django, it's called urls.py

```python
# -*- coding: utf-8 -*-

from django.conf.urls import patterns, include
from django.conf import settings

# Uncomment the next two lines to enable the admin:
from django.contrib import admin
admin.autodiscover()

urlpatterns = patterns('',
    # Example:
    # (r'^helloworld/', include('helloworld.foo.urls')),

    # Uncomment the admin/doc line below to enable admin documentation:
    (r'^admin/doc/', include('django.contrib.admindocs.urls')),

    # Uncomment the next line to enable the admin:
    (r'^admin/', include(admin.site.urls)),

    # Hello, world!
    (r'', 'helloworld.views.index'),
)
```

We can see that in that example, the routing of the site itself is configured in a list(?), on the first index of the urlpatterns, the line is actually stating that if the user go into the /admin/doc/ they will be served with the default admind documentation that are provided by Django itself
On the second index is quite obvious, it directs the user to the admin page (and user authentication is implemented here).
As at the last index, we have the line which route to the view that was mentioned before the index view.

---

