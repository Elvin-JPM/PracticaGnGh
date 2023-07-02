- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
R// > *git reset --hard <commit>*, porque al usar un reset --mixed se hubiese mantenido los cambios en el working copy.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
R// > *git reset --hard <commit-recuperado>*, porque si hago un git reset <commit-recuperado> no me trae los cambios que 
había realizado en el archivo git-nuestro.md.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
R// No hubo conflicto ya que el merge fue fast-forward al no haber bifurcaciones.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
R// Si hubo conflicto, porque en la rama htmlify se realizó cambios en el archivo git-nuestro.md en lineas que ya habian 
sido editadas en la rama styled.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
R// No causó conflicto, porque los archivos son idénticos dado que anteriormente se había hecho *merge* de style con 
main.

- ¿Qué comando o comandos utilizaste en el paso 25?
R//*git log --graph*

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
R// Si, porque entre el commit en el que se encuentra main y title no hay bifurcaciones.

- ¿Qué comando o comandos utilizaste en el paso 27?
R// *git reset <commit>*

- ¿Qué comando o comandos utilizaste en el paso 28?
R// *git reset --hard <commit>*

- ¿Qué comando o comandos utilizaste en el paso 29?
R// *git branch -D title*

- ¿Qué comando o comandos utilizaste en el paso 30?
R// *git reflog*, *git reset --hard <commit>*

- ¿Qué comando o comandos usaste en el paso 32?
R// *git reset <commit>*

- ¿Qué comando o comandos usaste en el punto 33?
R// *git reset --hard <commit>*

Para agregar los tags usé el comando: *git tag -a <tag-name> <commit> -m "message"*

Cuando me muevo a la etiqueta htmlify en el paso 35, entro en el estado *detached HEAD* y luego uso *git checkout main* 
para volver a la rama *main*.
