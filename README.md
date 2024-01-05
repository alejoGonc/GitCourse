# Git course

Este es un curso de Git y Github desde cero.

Para empezar vamos a necesitar isntalar Git en caso de que estemos trabajando en windows. Aquellos que esten trabajando con Mac o Linux no van a tener problemas.

Comandos Git:
- clone: hacer una copia de un repositorio que esta hosteado por ej en github a tu maquina local
- add: trackear tus archivos y cambios en git
- commit: guardas tus archivos en git
- push: subir tus commits a un repo remoto como github
- pull: descargar cambios desde un repo remoto a tu maquina local (el opuesto de push)

el workflow que se hace cuando trabajo localmente es el siguiente:
    - 1 Escribo el codigo nuevo
    - 2 git add
    - 3 git commit
    - 4 git push 

Que es el branching?
El branching permite crear nuevas ramas (branches) de codigo adicionales a la master o main. Esto permite crear nuevo codigo que no afecta a la rama principal, ya que son independientes. Los commits que hagas en una de las ramas no afectara a la otra.
Para que es útil esto? Bueno, cualquier nuevo feature, modificacion o prueba que quieras hacerle al codigo no va a romper al que ya funciona... sos libre para jugar. 
Tambien sirve para debuggear codigo sin trabajar sobre la rama principal, o para trabajar en equipos, etc.