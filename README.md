# P03---Git-local-a-remoto
Tarea de Entornos de Desarrollo


1. Comprueba la versión de Git

git --version

Comprueba tu usuario y correo configurados en Git

git config --global user.name
git config --global user.email


3. Crea una carpeta P03 dentro de tu carpeta local Entornos

cd ~/Entornos   # Ajusta si tienes otra ruta
mkdir P03


4. Métete en ella y muestra su contenido en formato largo y con archivos ocultos


cd P03
ls -la


5. Crea en esta carpeta un repositorio local


git init


6. Muestra el contenido del repositorio (incluye la carpeta .git)

ls -la


7. Crea un fichero con algún texto

echo "Este es el primer archivo" > archivo1.txt


8. Comprueba el estado del repositorio

git status


9. Añade el fichero al área de preparación (index)

git add archivo1.txt


10. Comprueba el estado del repositorio

git status


11. Confirma los cambios

git commit -m "Primer commit: añadir archivo1.txt"


12. Comprueba el estado del repositorio

git status


13. Añade otros dos ficheros

echo "Contenido archivo2" > archivo2.txt
echo "Contenido archivo3" > archivo3.txt


14. Comprueba el estado del repositorio

git status


15. Mételos en el área de preparación

git add archivo2.txt archivo3.txt


16. Comprueba el estado del repositorio

git status


17. Saca uno de los ficheros del área de preparación

git restore --staged archivo3.txt


18. Comprueba el estado del repositorio

git status


19. Añade el fichero que has eliminado del área de preparación al .gitignore

echo "archivo3.txt" >> .gitignore


20. Comprueba el estado del repositorio

git status


21. Si queda algo pendiente por añadir o confirmar, hazlo

git add .
git commit -m "Añadir archivo2 y .gitignore"


22. Comprueba el estado final del repositorio

git status


23. Muestra el registro de los cambios confirmados

git log --oneline


24. Sube el repositorio local a GitHub
Crea un nuevo repositorio vacío en GitHub llamado P03

Vincúlalo y sube el contenido:


git remote add origin https://github.com/TU_USUARIO/P03.git
git branch -M main
git push -u origin main
