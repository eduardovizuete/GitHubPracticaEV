- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
	git reset --hard HEAD~1
	este comando deshace el ultimo commit realizado y limpia el working copy

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
	git reflog
		este comando permite buscar el commit al que necesito regresas
	git checkout ebe0871
		este comando me permite regresar al commit que necesito

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
	Realizar el merge no causo conflicto, pero antes de cambiarse al branch styled se visualizo los siguientes avisos:
	
	git branch
		* (HEAD detached at ebe0871)
		  master
		  styled
	
	git checkout styled
		Warning: you are leaving 1 commit behind, not connected to
		any of your branches:
		ebe0871 Aniadir cambios git-nuestro.md paso 10
		If you want to keep it by creating a new branch, this may be a 			good time
		to do so with:
		git branch <new-branch-name> ebe0871
		Switched to branch 'styled'
	
	git branch
		  master
		* styled
	
	git merge master
		Already up-to-date.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
	No causo conflictos, se adjunta resultados
	
	git checkout styled
		Switched to branch 'styled'
		eduardo@eduardo-NV55C:$ git merge htmlify
		Updating fefc015..a362917
		Fast-forward
		 git-nuestro.md | 21 ++++++++++-----------
		 1 file changed, 10 insertions(+), 11 deletions(-)

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
	git checkout master
		Switched to branch 'master'
	
	git branch
		  htmlify
		* master
		  styled
	
	git merge styled
		Updating fefc015..a362917
		Fast-forward
		 git-nuestro.md | 21 ++++++++++-----------
		 1 file changed, 10 insertions(+), 11 deletions(-)

- ¿Qué comando o comandos utilizaste en el paso 25?

git graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

	Si, ya que el HEAD actual es un ancestro del commit que se esta
	tratando de hacer merge

- ¿Qué comando o comandos utilizaste en el paso 27?

	git reset --soft HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?

	git reset HEAD git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29?

	git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?

	git reflog
		este comando permite buscar el paso que se realizo el merge

	git checkout 7042280
		regresar al merge solicitado

- ¿Qué comando o comandos usaste en el paso 32?

	git reflog
		este comando permite buscar el commit inicial

	git checkout fefc015
		regresar al commit inicial

- ¿Qué comando o comandos usaste en el punto 33?

	git reflog
		este comando permite buscar el commit del titulo final

	git checkout 6209410
		volver al commit del titulo final