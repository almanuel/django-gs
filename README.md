# Django Getting Started
Taking notes. 

## Part 1 
`django-admin startproject mysite`
`python manage.py startapp <app-name>`

- Views and urls. 

## Part 2
- `settings.py`: Set timezone

- Database usage: 
`python manage.py migrate`

### Models
- Models Fields
- `settings.py` plug apps in `INSTALLED_APPS` variable.

### Migrations
- `makemigrations` command.
- `sqlmigrate` command
- `migrate` command.

### Shell
`python manage.py shell`

### Model CRUD operations on admin
Suppose a `polls` app and a `Question` model, on `polls/admin.py` file add: 
```python
from .models import Question
admin.site.register(Question)
```
That's it.

### Models API
- Queries, get, filters.`
## Part 3
- New views on new urls.
- Templates. [Read more here](https://docs.djangoproject.com/en/1.11/topics/templates/). 
- Raising 404 error
  - `raise django.http.Http404("Some message")`
  - Shortcuts: `get_object_or_404()` and `get_list_or_404()`
- Removing hardcoded URLs in templates, e.g:
```html
<a href="{% url 'detail' question.id %}">{{ question.question_text }}</a>
```
- Define app namespaces with `app_name` in `urls.py`. 






