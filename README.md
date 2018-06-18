# Practica Git Miguel Ángel Zamora


¿Qué comando utilizaste en el paso 11? ¿Por qué? 
-

```
git reset --hard HEAD~1
```

HEAD~1 para volver al commit anterior y --hard para deshacer los últimos cambios

¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 
-

```
git reflog 
```

Para obtener un histórico de todos los commits por los que me he movido con sus respectivos identificadores

```
git reset --hard 610f872
```

Vuelvo a usar este comando con el identificador del commit para volverme a él

El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
-

No, como la rama styled fue creada a partir de la rama master al intentar mergearla aparece *Already up-to-date* ya que tiene todos sus commits.

El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
-

Sí, hay un conflicto ya que estaban editadas las mismas líneas del mismo archivo, por lo tanto, tengo que resolver el conflicto a mano y luego volver a añadirlo y hacer un nuevo commit

El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
-

No, porque la rama styled contenía todos los commits de la rama master, desde la que fue creada, en caso de que la rama master hubiera tenido un nuevo commit independiente con cambios en ese fichero, entonces si hubiese existido un conflicto.

¿Qué comando o comandos utilizaste en el paso 25? 
-

```
git log --graph
```

También se le pueden añadir más opciones para que quede mas claro:

```
git log --graph --decorate --pretty=short
```

El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
-

Sí, ya que la rama title habia sido creada desde la rama master y contenía todos sus commits, sólo hacía falta mover el puntero de la rama master al último commit de la rama title

¿Qué comando o comandos utilizaste en el paso 27?
-

```
git reset HEAD~1
```

Uso git reset para volver al commit anterior, esta vez no le añado el --hard para poder conservar los últimos cambios

¿Qué comando o comandos utilizaste en el paso 28?
-

```
git checkout --git-nuestro.md
```

git checkout -- file para descartar los cambios del working directory

¿Qué comando o comandos utilizaste en el paso 29?
-

```
git branch -D title
```

La opción -D para eliminar ramas

¿Qué comando o comandos utilizaste en el paso 30?
-

```
git reflog
```

Para ver el histórico de commits volví a usar *git reflog* y luego vuelvo al commit con su identificador

```
git reset --hard 7a1ef2c
```



¿Qué comando o comandos usaste en el paso 32?
-

Vuelvo a necesitar ver los commits con sus identificadores

```
git reflog
```

Y esta vez uso git checkout para moverme por los commits

```
git checkout cac062e
```

¿Qué comando o comandos usaste en el punto 33?
-

```
git checkout 7a1ef2c
```