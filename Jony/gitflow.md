git branch *nombre de rama* - - - > crear rama

- - -
git checkout *nombre de rama*  - - - > moverme a esa rama

- - - 
git push origin *nombre de rama* - - - > PUSH 


- - - 
git merge *nombre de rama* - - > parado en la rama master o main y ejecutando ese comando, unimos esa rama a la rama master 

- - -
git rebase *nombre de rama*  --> Hacer rebase escencialmente selecciona un conjunto de commits, los "copia", y los aplica en algún otro lado.

- - - 
git rebase -i HEAD~*n de padres atras* o *nombre de la rama* - - - >
 
 Es el rebase interactivo. Git abrirá una UI para mostrarte qué commits están a punto de ser copiados sobre el objetivo del rebase. También muestra sus hashes y mensajes, que ayuda mucho para saber qué es cada commit. 
 
 - Puedes reordenar los commits con solamente cambiar su orden en la UI (en nuestra ventana, eso significa hacer drag & drop con el mouse).
 
 - Puedes elegir ignorar completamente algunos commits. Esto se designa con pick -- no hacerle pick a algún commit significa que quieres ignorarlo.

 - Finalmente, puedes squashear commits.

- - -
git cherry-pick *nombre de cada commit que desee copiar*

Es una manera bastante directa de decir que quieres copiar una serie de commits sobre tu ubicación actual (HEAD).

- - - 
git reset HEAD~*n de padres* --> deshace los cambios moviendo la referencia de una rama hacia atrás en el tiempo a un commit anterior. En este sentido puedes imaginarlo como "reescribir la historia". git reset va a mover la rama hacia atrás, como si el commit nunca se hubiera hecho. Su método de "reescribir la historia" no funciona para ramas remotas que otros están usando.

- - -
git revert --> Para revertir cambios y compartir esa revertida con otros, necesitamos usar git revert. 