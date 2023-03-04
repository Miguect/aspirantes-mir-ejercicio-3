PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1> md mision_s3


    Directorio: C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----      3/03/2023  6:51 p. m.                mision_s3


PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1> cd mision_s3
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git init
Initialized empty Git repository in C:/Users/Migue y Chris/Desktop/Ejercicios/Ejercicio1/mision_s3/.git/
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git add index.html
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git commit -m "añadiendo el archivo .html con información"
[master (root-commit) f5bce0c] añadiendo el archivo .html con información
 1 file changed, 1 insertion(+)
 create mode 100644 index.html
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git branch develop
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git checkout develop
Switched to branch 'develop'
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git branch
* develop
  master
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git add .gitignore
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git add index.html
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git commit -m "cambios en la rama develop"
[develop e37ba16] cambios en la rama develop
 2 files changed, 3 insertions(+), 1 deletion(-)
 create mode 100644 .gitignore
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git checkout main
error: pathspec 'main' did not match any file(s) known to git
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git checkout master
error: Your local changes to the following files would be overwritten by checkout:
        .gitignore
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git status
On branch develop
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git branch
* develop
  master
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git checkout master
error: Your local changes to the following files would be overwritten by checkout:
        .gitignore
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git add .gitignore
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git commit -m "otro commit por que no había guardado la información en el .gitignore jeje"
[develop dc37104] otro commit por que no había guardado la información en el .gitignore jeje
 1 file changed, 1 insertion(+)
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git status
On branch develop
nothing to commit, working tree clean
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git checkout master
Switched to branch 'master'
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> type index.html
Poniendo a prueba los conocimientos realizando la mision preparada por Make It Real
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git merge develop
Updating f5bce0c..dc37104
Fast-forward
 .gitignore | 1 +
 index.html | 4 +++-
 2 files changed, 4 insertions(+), 1 deletion(-)
 create mode 100644 .gitignore
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> type index.html
Poniendo a prueba los conocimientos realizando la mision preparada por Make It Real

AÃ±adiendo informaciÃ³n para el nuevo commit.
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> git ls-files --other --ignored --exclude-standard
.env


//este es el repositorio clonado y los comandos usados son los siguientes:
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1> cd mision_s3
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3> cd aspirantes-mir-ejercicio-3
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git init
Reinitialized existing Git repository in C:/Users/Migue y Chris/Desktop/Ejercicios/Ejercicio1/mision_s3/aspirantes-mir-ejercicio-3/.git/
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git status
On branch nueva-funcionalidad
nothing to commit, working tree clean
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git status
On branch nueva-funcionalidad
nothing to commit, working tree clean
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git branch
  master
* nueva-funcionalidad
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git add nuevo-archivo.txt
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git commit -m "commit en rama nueva-funcionalidad"
[nueva-funcionalidad 6d9c2d4] commit en rama nueva-funcionalidad
 1 file changed, 1 insertion(+)
 create mode 100644 nuevo-archivo.txt
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
PS C:\Users\Migue y Chris\Desktop\ejercicios\ejercicio1\mision_s3\aspirantes-mir-ejercicio-3> git merge nueva-funcionalidad
Updating b7638fc..6d9c2d4
Fast-forward
 nuevo-archivo.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 nuevo-archivo.txt
