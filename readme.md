
- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
	- Utilicé "git reset --hard HEAD~1"
	- Porque pide que perdamos los cambios realizados también en el "working copy" asi que con "hard" se hace directamente en un paso.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
	- Utilicé "git reset (SHA hash)"
	- Porque al utilizar "git reflog" observé dónde hice ese cambio y el comando reset "mueve" HEAD y la rama en la que estamos al "commit" que le indiques con alguna referencia ya que los "commits" nunca desaparecen y en ese "commit" es donde estaba antes de hacer el punto 11.

- El merge del paso 13, ¿causó algún conflicto? ¿Por qué?
	- No
	- Porque me aparece "already up to date" que significa que los cambios de la rama que intento fusionar ya se fusionaron con la rama en la que estoy actualmente. Concretamente significa que la rama que estoy fusionando es "un padre de su rama actual" y que no ha habido nuevos cambios en el padre desde la última fusión.

- El merge del paso 19, ¿causó algún conflicto? ¿Por qué?
	- Si
	- Porque he modificado el mismo archivo en las mismas líneas desde diferentes ramas en distinta posición (commit), con lo cual da conflicto.

- El merge del paso 21, ¿causó algún conflicto? ¿Por qué?
	- No
	- Porque con "merge" he absorbido todos los cambios a los que tiene acceso "styled" y al estar en el commit que ya de por sí tenía la información de todos los cambios no ha surgido ningún conflicto.

- ¿Qué comando o comandos utilizaste en el paso 25?
	- Utilicé "git log --graph" (Que no me aparecía en el diagrama el "commit" donde puse título ya que estaba posicionado en "master" como el ejercicio indica).

- El merge del paso 26, ¿podría ser fast-forward? ¿Por qué?
	- Si.
	- Porque no perdería ningún "commit" al hacer fast forward, seguiría teniendo acceso a todos los "commits" desde la posición donde se encuentra "title"

- ¿Qué comando o comandos utilizaste en el paso 27?
	- Utilicé "git reset HEAD~1"

- ¿Qué comando o comandos utilizaste en el paso 28?
	- Utilicé "git restore git-nuestro.md"

- ¿Qué comando o comandos utilizaste en el paso 29?
	- Utilicé "git branch -D title"

- ¿Qué comando o comandos utilizaste en el paso 30?
	- Utilicé "git reset (SHA hash)"

- ¿Qué comando o comandos usaste en el paso 32?
	- Utilicé "git reset --hard (SHA hash)"

- ¿Qué comando o comandos usaste en el punto 33?
	- Utilicé "git reset (SHA hash) + git restore git-nuestro.md" para conservar el título y todos los cambios realizados con anterioridad.
