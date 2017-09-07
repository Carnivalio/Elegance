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

[Pomodoro](https://en.wikipedia.org/wiki/Pomodoro_Technique) is a time management technique that was founded on 1980s, in this week of the task, to continue making my focus better combined with the task I've choosen last week, I decided to use this technique on myself, because I feel like I'm really easy to get distracted, I tried many of technique already but none of them actually made me work through my objective better than this pomodoro technique, it might be because of the rest time, so basically here's what I did:
On the first three days this pomodoro technique doesn't really affect my so called habit, I still tend to wander around while doing my work, but on the fourth day, I actually feel that this pomodoro helped me quite much, I can see that I finish more work than before I used this technique, I mean, it's just 25 minutes, it's not that much, but it actually does much.
Week before, I was planning to implement the anagram word search for my research, but I finished it in 3 days, because I wander a lot (especially on the web), but with this (and the commitment to not to wander, it's just 25 minutes anyway, right?) that kind level of task actually finished in a day!
It's not really that shocking for me, since I realize that I can be easily distracted, but this is the first time that I actually tried this technique and gained something out of it, I recommend people who like to 'delay' their work do this technique as well with 'it's easy, just 1 session of 25 minutes of focus' then you're good to go, you won't know what will this small technique will do to you.
