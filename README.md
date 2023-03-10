# web-personal
Proyecto en Django que muestra una web con información personal como el portafolio, contacto y redes sociales.

# Creando el entorno virtual
```sh
python3 -m venv env
cd web-personal
source env/bin/activate
# Windows
.\env\Scripts\activate
```

# Creando Proyecto web-personal
```sh
pip install django
pip install django-ckeditor
pip install Pillow
pip install pylint
pip install pylint-django
pip install pylint-celery

pip freeze > requirements.txt
```

```sh
# activar el entorno virtual 
source env/bin/activate

# Crear el proyecto con nombre app
django-admin startproject webpersonalapp
cd webpersonalapp/
# Crear o modificar la BD
python3 manage.py migrate
# Ejecutar el proyecto
python3 manage.py runserver
```

# Crear una aplicación dentro del proyecto
```sh
# activar el entorno virtual 
source env/bin/activate

cd webpersonalapp/
# crear aplicación core
python3 manage.py startapp core
```

# Hacer las migraciones de los modelos
```sh
# activar el entorno virtual 
source env/bin/activate

cd webpersonalapp/
python3 manage.py makemigrations core
python3 manage.py migrate

cd webpersonalapp/
python3 manage.py makemigrations portfolio
python3 manage.py migrate portfolio
```
```

# Crear un súper usuario
```sh
# activar el entorno virtual 
source env/bin/activate

python3 manage.py createsuperuser
```
