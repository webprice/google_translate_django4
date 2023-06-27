# Google Translate for Django 4 and Django 4+
## This is the working google translate library for Django v4 and above. 
> The orignal source and credits go to: https://pypi.org/project/django-google-translate/ (not working with Django 4+)

## Quick start
##### Download the package:
```
pip install django-google-translate
```
##### Add `google_translate` to your INSTALLED_APPS setting like this:
```
INSTALLED_APPS = [
    ...
    'google_translate',
]
```
##### Load the translate tag in your template (ideally on base.html):
```
{% load google_translate %}
``` 
##### Add following template tag wherever you want to show translate button:
```
{% google_translate %}
```
##### You can also pass type and default language in the translate button type in the inclusion tag (OPTIONAL):
```
{% google_translate type='vertical' language='en' %}
```
##### Available values for the type are "horizontal", "vertical" and "simple" (default) and for language you can pass any ISO language code