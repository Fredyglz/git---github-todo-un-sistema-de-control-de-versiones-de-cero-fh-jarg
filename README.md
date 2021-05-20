# GIT + GitHub: Todo un sistema de control de versiones de cero - Curso

En este repositorio podras encontrar todos los codigos y proyectos desarrollados en el curso de 'GIT + GitHub: Todo un sistema de control de versiones de cero' con Fernando Herrera disponible en la plataforma de Udemy lo cuales estaran divididos por secciones.

## Git - Fundamentos
**_Código:_** demo 01: https://github.com/Fredyglz/git-demo-01, demo 02: https://github.com/Fredyglz/git-demo-02

## APUNTES

### Comados  

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
