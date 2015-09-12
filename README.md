# exercises1Repositorio del Ejercicio1 de la practica

Respuesta Paso 11:
------------------
git reset --hard HEAD~1: Para que el WORKING COPY se quede igual que el REPO


Respuesta Paso 12:
------------------
git reflog
git reset --hard 980e799: Para mover al commit que se deshace en el paso11 y que el WORKING COPY recupere en el fichero poem.md la informción que tiene en el REPO de ese commit


Respuesta Paso 13:
------------------
git merge master: No existe conflicto.
Nos indica “already up-to-date” ya que la rama actual está al día, y no hay trabajo que absorber 


Respuesta Paso 19:
------------------
Si que aparecen conflictos ya que se había modificado el mismo fichero la misma linea en ramas diferentes (htmlify y matrix).


Respuesta paso 21:
------------------
No aparecen conflictos. La rama master sólamente tiene que absorver los cambios que se habían realizado en la rama htmlife. Se produce un merge fast foward.


Respuesta paso 25:
------------------
Se crea un alias con git config alias.graph "log --graph --decorate -- pretty=oneline"
Luego se ejecuta git log --graph 


Respuesta Paso 26:
------------------
El merge podría haber sido perfectamente fast foward ya que los commits que se quieren mergear están en linea.


Respuesta Paso 27:
------------------
git reset HEAD~1


Respuesta Paso 28:
------------------
git checkout -- poem.md


Respuesta Paso 29:
------------------
Se intenta primero con git branch -d title. Se nos indica que existe en esa rama un merge pendiente por lo que se procede a ejecutar git branch -D title (forzando el borrado).


Respuesta Paso 30:
------------------
Nos desplazamos al merge deshecho con git reset 075837a (donde se añadía el título). Como existen modificaciones pendientes pero no se ha perdido el trabajo con 
git checkout -- poem.md, se descartan los cambios que se proponen y se recupera el titulo que se creo en ese commit.


Respuesta Paso 32:
------------------
git checkout 6e00215 (hash del commit inicial donde se crea el fichero poem.md)


Respuesta Paso 33:
------------------
git checkout 075837a (hash del commit final donde se crea el titulo del fichero)

