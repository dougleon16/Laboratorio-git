# Introduccion a Git
## ¿Que es git?
Es un sistema de control de versiones y se utiliza para versionar software personal y de forma colaborativa.

## Comandos basicos en Git
1. `git init`: Inicializar un repositorio git.

``` bash
git init
```
2. `git add [archivo]`: agregar **archivo** al repositorio. Al Utilizar un punto (.), agregariamos todo los archivos
de nuestro directorio hacia nuestro repositorio.

``` bash
git add .
```
3. `git commit`: se utiliza para guardar los cambios realizados en la rama, junto con un mensaje preciso del commit

``` bash
git commit -m
```

4. `git diff`: diferencias entre archivo actual y su ultima version guardada  | diff <hash> archivo o <head> si no le doy el hash me manda al head es commit mas reciente.

``` bash
git diff <hash>
```
5. `git status`
6. `git branch` <nombre de la rama> crear un nueva rama
7. `git checkout` <nombre de la rama> para cambiar a la nueva rama


## Merge

git merge <nombre de la rama> para fusionar la nueva branch con la rama princiapl del repositorio

## volver en el tiempo
 1. git checkout <id del commit>
 2. git merge <rama a fusionar>
 revertir cambios realizados en un commit especifico:
 - git revert <id commit> regrese un cambio anterior a ese mismo branch, commit delante sigue existiendo, quedan en el stagin area
 - git reset te permite deshacer cambios sin crear un nuevo commit, util varios cambios en un solo comnado

## Maneras de crear un branch
`git branch [name]`
`git checkout -b [name]`

## Merge entre rama y resolucion de conflictos
 * El merge se puede hacer de forma manual y automatica 
 * si git detecta los cambios en las dos ramas no inteerfieren entre, el merge se puede realizar automaticamente 
 * si hay confilicros git pedira al usuario que resuelva los conflictos

