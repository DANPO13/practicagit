- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Utilice el comando "git reset --hard HEAD~1". Empleé este comando porque git reset te permite deshacer un commit o regresar a otro. Al añadirle la variante HEAD~1 deshací el commit anterior, pero como también tenía que perder los datos del working copy le incluí el --hard para hacer un retroceso más fuerte.
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Usé el comando "git reflog". Éste, funciona a modo de historial. Una vez lo activas te muestra todos los commits que has hecho aún habiéndolos deshechado. Para volver al commit que había quitado solo tenía que copiar el identificador que habia delante de este dentro de git reflog, y luego escribir el comando "git reset --hard (identificador)".
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

Si, ponía que ya estaba actualizado cuando no era así. No se podía hacer el merge porque estaba intentando que una rama hijo, que tiene más datos añadidos y los mismos que la otra, absorbiera a la rama madre.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?


Si, porque al haber editado el mismo archivo en las mismas líneas en las mismas ramas del mismo repositorio git se produce un conflicto de combinación al intentar fusionarlas. Para eso hay que realizar ciertos cambios en el archivo md. Caundo se abre se archivo surgen <<<<< HEAD que pertenece a la rama actual y >>>> perteneciente a la rama con la cual queremos que se fusione. Estos elementos deben borrarse y realizar los cambios pertinentes. Como el ejercicio pedía que mantuviera los cambios de la rama styled simplemente borré el trozo de texto con los cambios de htmlify.
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, porque la rama master y la rama styled tienen varias diferenciaciones en cuanto a los commits o los cambios del archivo md. Además la rama master es la madre de la rama styled.
- ¿Qué comando o comandos utilizaste en el paso 25?

El comando git log --graph.
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si, simplemente poniendo git merge sin el comando --no-ff que es el que indica que sea fast forward. La diferencia que hay entre uno y otro es que el merge fast forward no permite hacer un commit y el no ff sí.

- ¿Qué comando o comandos utilizaste en el paso 27?

Con el comando git reset HEAD~1 para volver un paso atrás sin remover el working copy.
- ¿Qué comando o comandos utilizaste en el paso 28?

El comando reflog, copio el identificador del punto a donde quiero ir y luego con el git reset (identificador).
- ¿Qué comando o comandos utilizaste en el paso 29?

El comando git branch -d nombre-rama. En este caso para eliminar la rama title tenía que hacer un borrado forzado ( -D ).
- ¿Qué comando o comandos utilizaste en el paso 30?

Pues el comando git reflog para copiar el identificador del merge y luego poniendo git reset --hard y pegar este.
 - ¿Qué comando o comandos usaste en el paso 32?

Empleé los comandos git reflog y git checkout para trasladarme al commit por medio del identificador.
- ¿Qué comando o comandos usaste en el punto 33?

Empleé los comandos git reflog y git checkout para trasladarme al commit por medio del identificador.