# GIT Cheat Sheet

Git es el sistema de control de versiones distribuido de código abierto que facilita las actividades de GitHub en su computadora portátil o de escritorio. Esta Cheat Sheet resume las instrucciones de línea de comando Git de uso común para una referencia rápida.

## Configurar Git

Definir el nombre a asignado a los commits.
`git config --global user.name "[name]"`

Definir el e-mail asignado a los commits
`git config --global user.email "[email address]"`

## Crear repositorios

Crear un repositorio local con un nombre
`git init [project-name]`

Descargar un proyecto y su historial de versiones
`git clone [url]`

## Hacer cambios

Listar los archivos nuevos o cambios
`git status`

Mostrar la diferencias que aún no han sido versionados
`git diff`

Agregar archivos o cambios para ser versioandos
`git add [file]`

Deshacer los cambios locales de un archivo
`git reset [file] `

Guardar los cambios en un commit
`git commit -m "[descriptive message]"`

## Cambios grupales

Listar todas las ramas locales en el repositorio actual
`git branch`

Crear una nueva rama
`git branch [branch-name]`

Cambiar a una rama y actualizar el directorio de trabajo
`git checkout -b [branch-name]`

Combinar una rama especificada con la actual
`git merge [branch-name]`

Eliminar una rama
`git branch -d [branch-name]`

## Refactorizar archivos

Eliminar un archivo en local y el repositorio
`git rm [file]`

Cambiar el nombre de un archivo en local y en el repositorio
`git mv [file-original] [file-renamed]`

## Guardar cambios locales sin hacer commit

Guardar temporalmente los archivos modificados
`git stash`

Restaurar los cambios más recientes almacenados temporalmente
`git stash pop`

Listar todos los conjuntos almacenados temporalmente
`git stash list`

Eliminar los cambios más recientes almacenados temporalmente
`git stahs drop`

## Deshacer Commits

Deshacer todos los commits despues de [commit], manteniendo los cambios locales
`git reset [commit]`

Deshacer la historia y cambios al commit especifcado
`git reset --hard [commit]`

## Sincronizar cambios

Subir todos los commits de un branch a GitHub
`git push [alias] [branch]`

Descargar todos los cambios e historial
`git pull`
