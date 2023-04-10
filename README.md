Git init

# start .
Verificamos que se creo el init - carpeta oculta

# creamos el gitignore
touch .gitignore
recordar pocolocar venv en el archivo para que no lo tome 
Recordar no hacer el commit antes ya que sino no lo va a tomar

# Creamos el entorno virtual
python -m venv venv

# instalamos django

# creamos el requirements.txt
pip freeze > requirements.txt

# Creamos la carpeta del proyecto pero sin necesidad de eliminala
django-admin startproject "Nombre"
django-admin startproject "after_project ."

# Corremos el servidor
python manage.py runserver

# Migramos
python manage.py migrate

Agregamos "db.sqlite3" en el gitignore