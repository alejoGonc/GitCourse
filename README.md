# Repo en proceso!!

# Git course

Este es un curso de Git y Github desde cero.

Para empezar vamos a necesitar isntalar Git en caso de que estemos trabajando en windows. 
Aquellos que esten trabajando con Mac o Linux no van a tener problemas.

Comandos principales de Git:
- clone: Hacer una copia de un repositorio que esta hosteado, por ejemplo en github, a tu maquina local.
- add: Trackear tus archivos y cambios en git.
- commit: Guardar (confirmar) tus cambios de archivos en git.
- push: Subir tus commits a un repo remoto como github.
- pull: Descargar cambios desde un repo remoto a tu maquina local (el opuesto de push)

El workflow que se hace cuando trabajas localmente es el siguiente:
     1. Escribo el codigo nuevo
     2. git add (hago el stage de los cambios)
     3. git commit (confirmo lso cambios)
     4. git push (mando los cambios al host, en mi caso Github)

Que es el branching?
El branching permite crear nuevas ramas (branches) de codigo adicionales a la master o main. Esto permite crear nuevo codigo que no afecta a la rama principal, ya que son independientes. Los commits que hagas en una de las ramas no afectara a la otra.
Para que es útil esto? Bueno, cualquier nuevo feature, modificacion o prueba que quieras hacerle al codigo no va a romper al que ya funciona... sos libre para jugar. 
Tambien sirve para debuggear codigo sin trabajar sobre la rama principal, o para trabajar en equipos, etc.

git branch: muestra las distintas ramas que existen y en cual estas posicionado, se ve con un asterisco

git checkout -b nombre-rama-nueva: crea una nueva rama dentro de tu repo y te posiciona en ella

git checkout nombre-rama: switchea entre ramas

git diff nombre-rama: me muestra las diferencias del codigo entre las ramas

git merge nombre-rama-nueva: hace el merge a la rama en la que estas parado de los cambios de la rama nueva

demo pull request desde github

pull request (pr) es basicamente un pedido para tener tu codigo pulleado en otra rama. Una vez que hacemos el pr, cualquera puede ver nuestro codigo, comentarlo o pedirnos que hagamos algun update

quick test changes
1
