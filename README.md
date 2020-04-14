<p align="center"><img src="https://github.com/romerojoseing/archivos/blob/master/img/logov.png?raw=true" width="150"></p>

<p align="center">
Te doy la bienvenida a mi repositorio, puedes usar este contenido con total libertad, siempre teniendo el mayor respeto por los autores que desarrollaron el proyecto.
</p>

<br>

# Curso Básico de Git y GitHub

<br>

## ¿Qué es Git?

Git es el sistema de control de versiones más popular del mundo, quiere decir que es el sistema que controla y administra las distintas versiones de un proyecto o programa. 

Puedes navegar por cada línea de código que has redactado, volviendo o revertir el código a una versión anterior que has desarrollado en el pasado. 

<br>

### Comandos de Git

Configurar Nombre de usuario
```
	git config --global user.name "romerojoseing"
```
Configurar Email
```	
  git config --global user.email "romerojoseing@gmail.com"
```

<br>

### Iniciando repositorio

Iniciamos Git en la carpeta del proyecto
```
	git init
```
Clonamos el repositorio de github, gitlab o bitbucket
```
	git clone <url>
```
Añadimos todos los archivos para el commit
```
	git add .
```
Hacemos el primer commit
```
	git commit -m "nombre del commit"
```
Subimos el proyecto al repositorio remoto
```
	git push origin master
```

<br>

### Git CLONE

Clonamos el repositorio de github, gitlab o bitbucket
```
	git clone <url>
```

<br>

### Git ADD

Añadimos todos los archivos para el commit
```
	git add .
```
Añadimos el archivo para el commit
```
	git add <archivo>
```
Añadimos todos los archivos con la extensión especificada
```
	git add *.txt
```
Añadimos todos los archivos dentro de un directorios
```
	git add docs/
```
Añadimos todos los archivos dentro de un directorio y de una extensión especifica
```
	git add docs/*.txt
```

<br>

### Git COMMIT

Cargar en el HEAD los cambios realizados
```
	git commit -m "cambios realizados"
```
Agregar y Cargar en el HEAD los cambios realizados
```
	git commit -a -m "cambios realizados"
```
De haber conflictos los muestra
```
	git commit -a 
```

<br>

### Git PUSH

Subimos todos los cambios
```
	git push
```
Subimos al repositorio
```
	git push <origien> <branch>
```

<br>

### Git LOG

Muestra los logs de los commits
```
	git log
```
Muestras los cambios detallados en los commits
```
	git log --oneline --stat
```
Muestra los nombres de los commits
```
	git log --oneline --graph
```

<br>

### Git DIFF

Muestra los cambios realizados a un archivo
```
	git diff
	git diff --staged
```

<br>

### Git HEAD

Saca un archivo del commit
```
	git reset HEAD <archivo>
```
Devuelve el ultimo commit que se hizo y pone los cambios en staging
```
	git reset --soft HEAD^
```
Devuelve el ultimo commit y todos los cambios
```
	git reset --hard HEAD^
```
Devuelve los 2 ultimo commit y todos los cambios
```
	git reset --hard HEAD^^
```
Rollback merge/commit
```
	git log
	git reset --hard <commit_sha>
```

<br>

### Git REMOTE

Agregar repositorio remoto
```
	git remote add origin <url>
```
Cambiar de remote
```
	git remote set-url origin <url>
```
Remover repositorio
```
	git remote rm <name/origin>
```
Muestra lista repositorios
```
	git remote -v
```
Muestra los branches remotos
```	
	git remote show origin
```
Limpiar todos los branches eliminados
```
	git remote prune origin 
```

<br>

### Git BRANCH

Crea un branch
```
	git branch <nameBranch>
```
Lista los branches
```
	git branch
```
Comando -d elimina el branch y lo une al master
```
	git branch -d <nameBranch>
```
Elimina sin preguntar
```
	git branch -D <nameBranch>
```

<br>

### Git TAG

Muestra una lista de todos los tags
```
	git tag
```
Crea un nuevo tags
```
	git tag -a <verison> - m "esta es la versión x"
```

<br>

### Git REBASE

Los rebase se usan cuando trabajamos con branches esto hace que los branches se pongan al día con el master sin afectar al mismo

Une el branch actual con el mastar, esto no se puede ver como un merge
```
	git rebase
```
Cuando se produce un conflicto no das las siguientes opciones:

cuando resolvemos los conflictos --continue continua la secuencia del rebase donde se pauso
```	
	git rebase --continue 
```
Omite el conflicto y sigue su camino
```
	git rebase --skip
```
Devuelve todo al principio del rebase
```
	git reabse --abort
```
Para hacer un rebase a un branch en especifico
```	
	git rebase <nameBranch>
```

<br>

### OTROS COMANDOS

Lista un estado actual del repositorio con lista de archivos modificados o agregados
```
	git status
```
Quita del HEAD un archivo y le pone el estado de no trabajado
```
	git checkout -- <file>
```
Crea un branch en base a uno online
```
	git checkout -b newlocalbranchname origin/branch-name
```
Busca los cambios nuevos y actualiza el repositorio
```
	git pull origin <nameBranch>
```
Cambiar de branch
```
	git checkout <nameBranch/tagname>
```
Une el branch actual con el especificado
```
	git merge <nameBranch>
```
Verifica cambios en el repositorio online con el local
```
	git fetch
```
Borrar un archivo del repositorio
```
	git rm <archivo> 
```

<br>

### Fork

Descargar remote de un fork
```
	git remote add upstream <url>
```

Merge con master de un fork
```
	git fetch upstream
	git merge upstream/master
```

<br>

## Tecnologías Usadas

- Git
- GitHub

<br><br>

## Autor

<p align="center"><img src="https://github.com/romerojoseing/archivos/blob/master/img/logoh.png?raw=true" width="200"></p>

<p align="center">
  Si te gusto el proyecto sígueme y dame apoyo para seguir creando más contenido.
</p>

<p align="center">
  <a target="_blank" href="https://romerojose.com/"><img src="https://github.com/romerojoseing/archivos/blob/master/img/web.png?raw=true" height="20"></a> - 
  <a target="_blank" href="https://www.linkedin.com/in/romerojoseing/"><img src="https://github.com/romerojoseing/archivos/blob/master/img/linkedin.png?raw=true" height="20"></a> - 
  <a target="_blank" href="https://github.com/romerojoseing"><img src="https://github.com/romerojoseing/archivos/blob/master/img/github.png?raw=true" height="20"></a> - 
  <a target="_blank" href="https://www.instagram.com/romerojoseing/"><img src="https://github.com/romerojoseing/archivos/blob/master/img/instagram.png?raw=true" height="20"></a> - 
  <a target="_blank" href="https://www.facebook.com/romerojoseing"><img src="https://github.com/romerojoseing/archivos/blob/master/img/facebook.png?raw=true" height="20"></a> - 
  <a target="_blank" href="https://twitter.com/romerojoseing"><img src="https://github.com/romerojoseing/archivos/blob/master/img/twitter.png?raw=true" height="20"></a>
</p>