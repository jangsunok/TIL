

## Slug & SlugField
Slug is a newspaper term. A slug is a short label for something, containing only letters, numbers, underscores or hyphens. They're generally used in URLs
- https://stackoverflow.com/questions/427102/what-is-a-slug-in-django
- https://keyerror.com/blog/automatically-generating-unique-slugs-in-django


## DateTimeFiled
- https://docs.djangoproject.com/ko/2.1/ref/models/fields/#datefield
### DateField.auto_now
1. Automatically set the field to now every time the object is saved. Useful for "last-modified" timestamps. Note that the current date is always used; it's not just a default value that you can override.
2. The field is only automatically updated when calling Model.save(). The field isn't updated when making updates to other fields in other ways such as QuerySet.update(), though you can specify a custom value for the field in an update like that.
### DateField.auto_now_add
1. Automatically set the field to now when the object is first created. Useful for creation of timestamps. Note that the current date is alwaysused; it's not just a default value that you can override. So even if you set a value for this field when creating the object, it will be ignored. If you want to be able to modify this field, set the following instead of auto_now_add=True:




## F() expressions
- https://docs.djangoproject.com/ko/2.0/ref/models/expressions/#f-expressions



## django.models.Signals
https://docs.djangoproject.com/en/2.1/topics/signals/
https://dgkim5360.tistory.com/entry/django-signal-example
