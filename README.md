# GIT + GitHub: Todo un sistema de control de versiones de cero - Curso

En este repositorio podras encontrar todos los codigos y proyectos desarrollados en el curso de 'GIT + GitHub: Todo un sistema de control de versiones de cero' con Fernando Herrera disponible en la plataforma de Udemy lo cuales estaran divididos por secciones.

## Git - Fundamentos
**_Código:_** demo 01: https://github.com/Fredyglz/git-demo-01, demo 02: https://github.com/Fredyglz/git-demo-02

## Un poco más allá de los fundamentos de GIT
**_Código:_** demo 03: https://github.com/Fredyglz/git-demo-03, demo 04: https://github.com/Fredyglz/git-demo-04, demo 05 - tarea: https://github.com/Fredyglz/git-demo-05

## Ramas, uniones, conflictos y tags
**_Código:_** demo 06: https://github.com/Fredyglz/git-demo-06

## Git Stash y Git Rebase - Para realizar cambios de emergencia  
**_Código:_** demo 07: https://github.com/Fredyglz/git-demo-07, demo 08: https://github.com/Fredyglz/git-demo-08

# Apuntes

## Comados  

### Fundamentos
**git --version**  
Sirven para saber la version de github que estamos utilizando

**git help**  
Despliega información sobre todos los comandos disponibles en git

**git help <nombre_comando\>**  
Despliega información espedifica sobre un comando en particular

**git config --global user.name <name\>**  
Sirve para guardar la configuración de manera global del nombre del usuario

**git config --global user.email <email\>**  
Sirve para guardar la configuración de manera global del correo del usuario

**git config --global -e**  
Sirve para mostrar toda la condiguración global guardada en modo escritura

**git config --global -l**  
Sirve para mostrar toda la condiguración global guardada en modo lectura

**git init**   
Crea un repositorio nuevo

**git status**  
Muestra el estado del repositorio y el área de preparación. Nos permite ver los archivos y cambios rastreados y no rastreados

**git status -s**  
Muestra el estado del repositorio y el área de preparación. Nos permite ver los archivos y cambios rastreados y no rastreados de manera mas corta

**git status -s -b**  
Muestra el estado del repositorio y el área de preparación. Nos permite ver los archivos y cambios rastreados y no rastreados de manera mas corta indicando la rama en la que nos encontramos

**git status -sb**  
Muestra el estado del repositorio y el área de preparación. Nos permite ver los archivos y cambios rastreados y no rastreados de manera mas corta indicando la rama en la que nos encontramos

**git add .**  
Agrega todos los archivos con cambios no registrados al area de preparación

**git add -A**  
Agrega todos los archivos con cambios no registrados al area de preparación

**git add --all**  
Agrega todos los archivos con cambios no registrados al area de preparación

**git add <nombre_archivo\>**  
Agrega unicamente el archivo especificado como parametro

**git add "\*.txt"**  
Agrega todos los txt de TODO el proyecto

**git add \*.txt**  
Agrega todos los txt en el directorio actual

**git add \*.png**  
Agrega todos los archivos con extensión .png

**git add pdfs/\*.pdf**  
Agrega todos los PDFs dentro de la carpeta PDFs

**git add pdfs/**  
Agrega todos los archivos dentro de la carpeta PDFs

**git reset \*.xml**  
Excluye del stage todos los archivos con terminación .xml

**git commit**  
Se utiliza para registrar los cambios en el repositorio.

**git checkout -- .**  
Reconstruye todo el proyecto a como estaba en el ultimo commit

**git log**  
Revisa y lee el historial de todo lo que le sucede al repositorio

**git log --oneline**  
Revisa y lee el historial de todo lo que le sucede al repositorio pero solo regresa el hash corto, la descripción de la rama y lo que se hizo en ese commit

**git log --oneline --decorate --all --graph**
Revisa y lee el historial de todo lo que le sucede al repositorio pero solo regresa el hash corto, la descripción de la rama y lo que se hizo en ese commit a detalle

**git config --global alias.<alias\> "<comando comando\>"**    
Configura alias para agreviar una lista de comandos en uno solo  
_Ej. git config --global alias.lg "log --oneline --decorate --all --graph"_

### Un poco mas allá de los fundamentos de GIT
**git diff**  
Muestra los cambios que hubo en los archivos antes de mandarlos al stage

**git diff --staged**  
Muestra los cambios que hubo en los archivos antes de mandarlos al stage

**git reset HEAD <nombre_archivo\>**  
Quita del stage al archivo especificado

**git checkout -- README.md**  
Reconstruye el archivo a como estaba en el ultimo commit

**git commit -am "<descripción_del_commit\>"**  
Agrega al stage y realiza el commit de los archivos de manera simultanea

**git --amend -m "<descripción_del_commit\>"**  
Restablecemos la descipcion del ultimo commit registrado

**git reset --soft HEAD^**  
Cambia mi HEAD a un commit anterior proximo dejando los cambios en el stage

**git reset --soft <hash_commit\>**  
Cambia mi HEAD a un commit con el hash especificado dejando los cambios en el stage

**git reset --mixed <hash_commit\>**  
Cambia mi HEAD a un commit con el hash especificado dejando los cambios antes de mandarlos al stage

**git reset --hard <hash_commit\>**  
Cambia mi HEAD a un commit con el hash especificado destruyendo los cambios agregados

**git reflog**  
Muestra todos los cambios en el tiempo registrados por git

**git mv <nombre_actual\> <nombre_nuevo>**  
Renombra un archivo manteniendo sus cambios

**git rm <nombre_actual\>**  
Elimina un archivo

**git add -u**  
Agrega al stage todos los archivos modificados y eliminados

### Ramas, uniones, conflictos y tags

**git branch <nombre_rama\>**  
Crea una nueva rama en el repositorio

**git branch**  
Lista el nombre de las ramas marcando con verde en la que me encuentro actualmente

**git checkout <nombre_rama\>**  
Me mueve a la rama seleccionada

**git diff <nombre_rama> <nombre_rama_2>**  
Muestra las diferencias entre las dos ramas

**git merge <nombre_rama_a_unir\>**  
Con este comando, primero tenemos que estar en la rama donde queremos que se unan las modificaciones viniendo de otra, esa otra seria la que se manda como parametro en el comando

**git branch -d <nombre_rama\>**  
Elimina la rama seleccionada, usualmente se usa cuando ya se realizo un merge con su contenido a otra rama y esta ya no se va a utilizar

**git checkout -b <nombre_rama\>**  
Crea una nueva rama y automaticamente me mueve a ella

**git tag <nombre_tag\>**  
Crea un nuevo tag

**git tag**  
Lista todos los tag creados

**git tag -d <nombre_tag\>**  
Elimina un tag especifico 

**git tag -a v<numero_version\> -m <mensaje>**  
Crea tags mas especificos

**git tag -a v<numero_version\> <hash_commit> -m <mensaje>**  
Crea tags mas especificos en un commit especifico

**git show <tag_anotado_(-a)>**  
Muestra los detalles de un tag especifico

### Git Stash y Git Rebase - Para realizar cambios de emergencia
**git stash**  
Permite cambiar de rama sin confirmar la rama actual.

**git stash save**  
Permite cambiar de rama sin confirmar la rama actual.

**git stash list**  
Lista todos los trabajos en progreso que hay

**git stash pop**  
Extrae el ultimo elemento del stack de stashes y lo elimina del mismo

**git stash apply**  
Extrae el ultimo elemento del stack de stashes y lo deja en la lista de stashes

**git stash apply stash@{<id\>}**  
Extrae un stash con id especifico del stack de stashes y lo deja en la lista de stashes

**git stash drop**  
Elimina el ultimo elemento del stack de stashes

**git stash drop stash@{<id\>}**  
Elimina un stash con id especifico del stack de stashes

**git stash save --keep-index**  
Guarda todo menos los archivos en el stage o en el escenario

**git stash save --include-untracked**  
Incluye todo los archivos, junto a los que git no le da seguimiento

**git stash list --stat**  
Muestra mas información de cada una de las entradas del stash

**git show stash**
Muestra mas informacion de los cambios de las lineas que se hizo en el ultimo stash

**git show stash@{<id\>}**
Muestra mas informacion de los cambios de las lineas que se hizo en el ultimo stash

**git stash save "<mensaje\>"**
Agrega mensajes a los stash

**git stash clear**  
Borra todas las entradas que hay en el stash

**git rebase <nombre_rama_a_rebasar\>**  
Se utiliza para aplicar una secuencia de confirmaciones de distintas ramas en una confirmación final

**git rebase -i HEAD~<numero_de_ultimos_commits_requeridos\>**  
Se utiliza para hacer un rebase interactivo 

**squash**  
Une los commits 

**reward**  
Edita el mensaje de los commits

**edit**  
Separa un commit

**git rebase --continue**  
Reasigna el HEAD
