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

if settings.DEBUG:
    urlpatterns += patterns('',
        (r'^media/(?P<path>.*)$', 'django.views.static.serve',
         {'document_root': settings.MEDIA_ROOT}),
)
```

We can see that in that example, the routing of the site itself
