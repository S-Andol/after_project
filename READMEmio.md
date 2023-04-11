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
Tambien "__pycache__"

# Generamos el commit
git status
git add .
git commit -m "Creación de la base del proyecto"


# cambiamos el nombre de la rama
git branch -M main

# Agregamos un remoto
git remote add origin https://github.com/S-Andol/after_project.git

este "origin" nos evita despues colocar todo el https... origin = alias

git remote -v

se cran:
origin  https://github.com/S-Andol/after_project.git (fetch) - Para traerse los cambios
origin  https://github.com/S-Andol/after_project.git (push) . Para subir los cambios

# Pusheamos
git push
copiamos y pegamos lo que nos dice
git push --set-upstream origin main (vemos que no nos deja)

Probamos con 
git push -u origin main (tampoco porque tenemos cambios en la nube)

Debemos traer los cambios de la nube, acomodas las cosas y listo... vamos a poder pushear

# Traemos los cambios
git pull
Vemos que tampoco lo tenemos configurado, hay que configurarlo...

git pull <remote> <branch>
git pull origin main

Nos va a tirar errores...

Fijate que podes tener errores en los gitignore como en los readme si los creaste antes. Cambiales el nombre al que te diga por pantalla

# Al profe no le salio
# Vamos a fetchear
git pull --allow-unrelated-histories

git pull y listo


