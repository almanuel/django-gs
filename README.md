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
```
from .models import Question
admin.site.register(Question)
```
That's it.

### Models API
- Queries, get, filters.


