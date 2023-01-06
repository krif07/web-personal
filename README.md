# web-personal
```sh
Proyecto en Django que muestra una web con información personal como el portafolio, contacto y redes sociales.
```
# Creando el entorno virtual
```sh
python3 -m venv env
cd web-personal
source env/bin/activate
```

# Creando Proyecto web-personal
```sh
pip install django

```

```sh
# Crear el proyecto con nombre app
django-admin startproject app
cd app/
# Crear o modificar la BD
python3 manage.py migrate
# Ejecutar el proyecto
python3 manage.py runserver
```

# Crear una aplicación dentro del proyecto
```sh
cd app/
# crear aplicación polls
python3 manage.py startapp polls
```

# Hacer las migraciones de los modelos
```sh
cd app/
python3 manage.py makemigrations polls
python3 manage.py migrate
```

# Crear un súper usuario
```sh
python3 manage.py createsuperuser

```