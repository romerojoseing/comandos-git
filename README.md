# Comandos de Git

<br>

## ¿Qué es Git? 👀

Git es el sistema de control de versiones más popular del mundo, quiere decir que es el sistema que controla y administra las distintas versiones de un proyecto o programa. 

Puedes navegar por cada línea de código que has redactado, volviendo o revertir el código a una versión anterior que has desarrollado en el pasado. 

<br>

## Configurar Git ⚙

Configurar Nombre de usuario
```ssh
	$ git config --global user.name "romerojoseing"
```
Configurar Email
```ssh
	$ git config --global user.email "romerojoseing@gmail.com"
```

<br>

## Iniciando repositorio ▶

Iniciamos Git en la carpeta del proyecto
```ssh
	$ git init
```
Clonamos el repositorio de github, gitlab o bitbucket
```ssh
	$ git clone <url>
```
Añadimos todos los archivos para el commit
```ssh
	$ git add .
```
Hacemos el primer commit
```ssh
	$ git commit -m "nombre del commit"
```
Subimos el proyecto al repositorio remoto
```ssh
	$ git push origin master
```

<br>

## Git CLONE 🎞

Clonamos el repositorio de github, gitlab o bitbucket
```ssh
	$ git clone <url>
```

<br>

## Git ADD ✔

Añadimos todos los archivos para el commit
```ssh
	$ git add .
```
Añadimos el archivo para el commit
```ssh
	$ git add <archivo>
```
Añadimos todos los archivos con la extensión especificada
```ssh
	$ git add *.txt
```
Añadimos todos los archivos dentro de un directorios
```ssh
	$ git add docs/
```
Añadimos todos los archivos dentro de un directorio y de una extensión especifica
```ssh
	$ git add docs/*.txt
```

<br>

## Git COMMIT 🎫

Cargar en el HEAD los cambios realizados
```ssh
	$ git commit -m "cambios realizados"
```
Agregar y Cargar en el HEAD los cambios realizados
```ssh
	$ git commit -a -m "cambios realizados"
```
De haber conflictos los muestra
```ssh
	$ git commit -a 
```

<br>

## Git PUSH ⬆

Subimos todos los cambios
```ssh
	$ git push
```
Subimos al repositorio
```ssh
	$ git push <origien> <branch>
```

<br>

## Git LOG 💾

Muestra los logs de los commits
```ssh
	$ git log
```
Muestras los cambios detallados en los commits
```ssh
	$ git log --oneline --stat
```
Muestra los nombres de los commits
```ssh
	$ git log --oneline --graph
```

<br>

## Git DIFF 💱

Muestra los cambios realizados a un archivo
```ssh
	$ git diff
	$ git diff --staged
```

<br>

## Git HEAD ❌

Saca un archivo del commit
```ssh
	$ git reset HEAD <archivo>
```
Devuelve el ultimo commit que se hizo y pone los cambios en staging
```ssh
	$ git reset --soft HEAD^
```
Devuelve el ultimo commit y todos los cambios
```ssh
	$ git reset --hard HEAD^
```
Devuelve los 2 ultimo commit y todos los cambios
```ssh
	$ git reset --hard HEAD^^
```
Rollback merge/commit
```ssh
	$ git log
	$ git reset --hard <commit_sha>
```

<br>

## Git REMOTE 📟

Agregar repositorio remoto
```ssh
	$ git remote add origin <url>
```
Cambiar de remote
```ssh
	$ git remote set-url origin <url>
```
Remover repositorio
```ssh
	$ git remote rm <name/origin>
```
Muestra lista repositorios
```ssh
	$ git remote -v
```
Muestra los branches remotos
```ssh
	$ git remote show origin
```
Limpiar todos los branches eliminados
```ssh
	$ git remote prune origin 
```

<br>

## Git BRANCH 🌱

Crea un branch
```ssh
	$ git branch <nameBranch>
```
Lista los branches
```ssh
	$ git branch
```
Comando -d elimina el branch y lo une al master
```ssh
	$ git branch -d <nameBranch>
```
Elimina sin preguntar
```ssh
	$ git branch -D <nameBranch>
```

<br>

## Git TAG 📌

Muestra una lista de todos los tags
```ssh
	$ git tag
```
Crea un nuevo tags
```ssh
	$ git tag -a <verison> - m "esta es la versión x"
```

<br>

## Git REBASE

Los rebase se usan cuando trabajamos con branches esto hace que los branches se pongan al día con el master sin afectar al mismo

Une el branch actual con el mastar, esto no se puede ver como un merge
```ssh
	$ git rebase
```
Cuando se produce un conflicto no das las siguientes opciones:

cuando resolvemos los conflictos --continue continua la secuencia del rebase donde se pauso
```ssh
	$ git rebase --continue 
```
Omite el conflicto y sigue su camino
```ssh
	$ git rebase --skip
```
Devuelve todo al principio del rebase
```ssh
	$ git reabse --abort
```
Para hacer un rebase a un branch en especifico
```ssh
	$ git rebase <nameBranch>
```

<br>

## OTROS COMANDOS 🕹

Lista un estado actual del repositorio con lista de archivos modificados o agregados
```ssh
	$ git status
```
Quita del HEAD un archivo y le pone el estado de no trabajado
```ssh
	$ git checkout -- <file>
```
Crea un branch en base a uno online
```ssh
	$ git checkout -b newlocalbranchname origin/branch-name
```
Busca los cambios nuevos y actualiza el repositorio
```ssh
	$ git pull origin <nameBranch>
```
Cambiar de branch
```ssh
	$ git checkout <nameBranch/tagname>
```
Une el branch actual con el especificado
```ssh
	$ git merge <nameBranch>
```
Verifica cambios en el repositorio online con el local
```ssh
	$ git fetch
```
Borrar un archivo del repositorio
```ssh
	$ git rm <archivo> 
```

<br>

## Fork

Descargar remote de un fork
```ssh
	$ git remote add upstream <url>
```

Merge con master de un fork
```ssh
	$ git fetch upstream
	$ git merge upstream/master
```

<br><br>

## Construido con 🛠️

_Para el desarrollo de este proyecto se utilizaron las siguientes tecnologías:_

* [Git](https://git-scm.com/) - Gestión y control de versiones.
* [GitHub](https://github.com) - Almacenamiento de repositorios en la nube.

<br>

## Autor ✒️

_Si te gusta lo que hago, visita mi web y comparte mi contenido, también puedes seguirme en mis redes para estar al tanto de nuevas publicaciones y proyectos interesantes que estaré desarrollando._

Diseñado con 💖 - por [Romero José](https://romerojose.com/)

### Redes Sociales

* **GitHub** - *Repositorios de mis últimos proyectos* - [romerojoseing](https://github.com/romerojoseing)
* **CodePen** - *Mini proyectos y pruebas interesantes* - [romerojoseing](https://codepen.io/romerojoseing)
* **LinkedIn** - *Perfil desarrollador profesional* - [romerojoseing](https://www.linkedin.com/in/romerojoseing/)
* **Instagram** - *Documentando mi viaje* - [romerojoseing](https://www.instagram.com/romerojoseing/)
* **Facebook** - *Publicaciones y contenido promocional* - [romerojoseing](https://www.facebook.com/romerojoseing)
* **Twitter** - *Comentarios random y más* - [romerojoseing](https://twitter.com/romerojoseing)