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

---

¿Qué es el branching?

El branching permite crear nuevas ramas (branches) de codigo adicionales a la master o main. Esto permite crear nuevo codigo que no afecta a la rama principal, ya que son independientes. Los commits que hagas en una de las ramas no afectara a la otra (a menos que hagas el merge).
Para que es útil esto? Cualquier nuevo feature, modificacion o prueba que quieras hacerle al codigo no va a romper al que ya funciona... sos libre para jugar. 
Tambien sirve para debuggear codigo sin trabajar sobre la rama principal, o para trabajar en equipos, etc.

---
Otros comandos útiles:
- git branch: muestra las distintas ramas que existen y en cual estas posicionado (marcada con un asterisco)
- git checkout -b nombre-rama-nueva: crea una nueva rama dentro de tu repo y te posiciona en ella.
- git checkout nombre-rama: switchea entre ramas.
- git diff nombre-rama: me muestra las diferencias del codigo entre las ramas.
- git merge nombre-rama-nueva: hace el merge a la rama en la que estas parado de los cambios de la rama nueva.
---
Pull Requests:

Pull request (pr) es basicamente un pedido para tener tu codigo pulleado en otra rama. Una vez que hacemos el pr, cualquiera puede ver nuestro codigo, comentarlo o pedirnos que hagamos algun update antes de hacer el merge a la rama.

---
Buenas prácticas y otros comentarios:

El commit perfecto: Mientras menos archivos incluya cada commit, mejor. Es importante saber que también se pueden hacer commits de solo algunas partes de los archivos, lo cual me sirve si quiero hacer un commit sobre un tema en específico.
Esto se puede hacer con: git add -p file-name. Git nos va a preguntar en que parte del archivo queremos hacer el stage y lo va a guardar en el commmit. Después hacemos el push normalmente.
Es importante ser descriptivos con los mensajes de los commits. Tiene que ser fácil diferenciar qué es distinto, y no debe ser repetitivo con los commits anteriores.
