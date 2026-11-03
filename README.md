# Proyecto de web personal en Django
Proyecto básico de introducción a Django, basado en la creación de una web sencilla con un portafolio dinámico y un panel de administración para manejar los proyectos del portafolio.
Basado en el curso [Curso Práctico de Django: Desarrollo Web Backend con Python](udemy.com/course/curso-django-2-practico-desarrollo-web-python-3/).

Conceptos utilizados:
- Estructura básica de un proyecto en Django
- División en aplicaciones
- Creación de páginas con HttpResponse
- Utilización de plantillas
- Plantillas con herencia
- Template tag url
- Carga de ficheros estáticos
- Template tag if y request.path
- Creación de modelos
- Personalización del panel de administración
- Patrón Modelo-Vista-Template
- Campos opcionales

## Instalación con Pipenv
- Instalación de paquetes
```bash
pipenv install django django-ckeditor Pillow pylint pylint-django pylint-celery
```

- Creación del proyecto
```bash
pipenv run django-admin startproject django-webpersonal
```

## Ejecución del proyecto
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

## Ampliando el proyecto
- Aplicación de las migraciones iniciales
```bash
python manage.py migrate
```

- Creación de una aplicación
```bash
python manage.py startapp core
```

## Creación de modelos
- Creación de una aplicación
```bash
python manage.py startapp portfolio
```

- Ejecución de la migración
```bash
python manage.py makemigrations portfolio
```

- Aplicación de la migración a la base de datos
```bash
python manage.py migrate portfolio
```

- Creación del superusuario
```bash
python manage.py createsuperuser
```
