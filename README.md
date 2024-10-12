# Desafío Guiado - Introducción a Django

Este proyecto es una aplicación web básica en Django que contiene tres vistas: **Home**, **About**, y **Contact**. Cada una de estas vistas muestra una página HTML simple, y en el caso de la vista **Contact**, incluye un formulario de contacto básico.

## Requisitos

Antes de comenzar, asegúrate de tener instalado lo siguiente:

- Python 3.x
- Django 5.0.2 (incluido en `requirements.txt`)

## Instalación

Sigue estos pasos para configurar el proyecto localmente:

1. Clona este repositorio en tu máquina local.
```bash
git clone <URL_DEL_REPOSITORIO>
```

2. Crea un entorno virtual.

```bash
python -m venv venv
```
3. Activa el entorno virtual:

Windows:
```bash
.\venv\Scripts\activate
```

macOS/Linux:
```bash
source venv/bin/activate
```

4. Instala las dependencias utilizando el archivo requirements.txt:
```bash
pip install -r requirements.txt
```

5. Ejecuta las migraciones de Django para aplicar los cambios de la base de datos:

```bash
python manage.py migrate
```

6. Inicia el servidor de desarrollo:

```bash
python manage.py runserver
```
Visita http://127.0.0.1:8000/ en el navegador para ver la aplicación en funcionamiento.

## Estructura del Proyecto
desafioGuiado/
├── desafioGuiado/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
├── viewsApp/
│   ├── __init__.py
│   ├── views.py
│   ├── migrations/
│   └── ...
├── templates/
│   ├── home.html
│   ├── about.html
│   ├── contact.html
└── manage.py


## Vistas
Home: Muestra una página de bienvenida con un texto de prueba generado con Lorem Ipsum.
About: Proporciona información básica sobre el sitio.
Contact: Incluye un formulario de contacto simple con campos para el nombre, correo electrónico y mensaje.


## Configuración de Templates
Los archivos HTML para las vistas están en la carpeta templates. 
Se utilizan las rutas estándar para renderizar estos templates desde las vistas en viewsApp/views.py.

## Uso
Home: http://127.0.0.1:8000/
About: http://127.0.0.1:8000/about/
Contact: http://127.0.0.1:8000/contact/


## Dependencias
Las dependencias están especificadas en el archivo requirements.txt:

asgiref==3.7.2
Django==5.0.2
sqlparse==0.4.4
tzdata==2024.1


## Autor

Bárbara HA.