# Proyecto de web personal en Django
Proyecto básico de introducción a Django, basado en la creación de una web sencilla con un portafolio dinámico y un panel de administración para manejar los proyectos del portafolio.
Basado en el curso [Curso Práctico de Django: Desarrollo Web Backend con Python](udemy.com/course/curso-django-2-practico-desarrollo-web-python-3/).

## Instalación con Pipenv
- Instalación de paquetes
```bash
pipenv install django django-ckeditor Pillow pylint pylint-django pylint-celery
```

- Creación del proyecto
```bash
pipenv run django-admin startproject django-webpersonal
```

# Ejecución del proyecto
- Ejecución directa
```bash
pipenv run python django-webpersonal/manage.py runserver
```

- Añadiendo script en Pipfile
```bash
[scripts]
webpersonal = "python django-webpersonal/manage.py runserver"
```

La ejecución se realiza con:
```bash
pipenv run webpersonal
```

- Aplicación de las migraciones iniciales
```bash
python manage.py migrate
```

- Creación de una aplicación
```bash
python manage.py startapp core
```