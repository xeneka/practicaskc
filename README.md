# Práctica GIT
**- ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

El comando que he utilizado es git reset —hard HEAD~1
Porque retrocede un comit y deja el working copy como estaba en el commit al que retrocedo.

**- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

Utilice reflog para poder ver cual es el commit al que tengo que volver. Una vez localizado el hash del commit al que quiero llegar git reset —hard hash. Lo utilizo hard para que me restaure al working copy al mismo que tiene el commit

**- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No causo ningún conflicto porque el commit de master ya era parte de esa rama.

**- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Si ha conflictos porque el contenido del fichero en cada uno de los commit es distintos. Me quedo con el que dice el enunciado y hago el commit

**- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No ha causado ningún conflicto fue un merge fast forward con el padre

**- ¿Qué comando o comandos utilizaste en el paso 25?**

git log --graph --decorate

**- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?** 

Si, porque esta en la misma lista

**- ¿Qué comando o comandos utilizaste en el paso 27?**

git reset HEAD~1 . También podría haber utilizado git reflog y utilizar el hash del commit padre para hacer un git reset hash. Como no quiero perder los cambio en el working copy no uso ni git reset —hard ni checkcout

**- ¿Qué comando o comandos utilizaste en el paso 28?** 
Entiendo que es descartar los cambios del working copy. Utilizo git checkout — git-nuestro.md

**- ¿Qué comando o comandos utilizaste en el paso 29?** 

git branch -D title como no esta mergeada uso la D en lugar de d

**- ¿Qué comando o comandos utilizaste en el paso 30?**

git reflog para ver el hash y git reset —hard hash para volver al punto donde estaba y recuperar el working copy que había en ese commit.

**- ¿Qué comando o comandos usaste en el paso 32?**

git reflog para ver los hash (en este caso a633ef5)
git checkout a63ef5

**- ¿Qué comando o comandos usaste en el punto 33?**

git reflog  para saber el hash en este caso dc92387
git checkout dc92387
