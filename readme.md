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

## Merge netre rams y resolucion de conflictos
 * El merge se puede hacer de forma manual y automatica 
 * si git detecta los cambios en las dos ramas no inteerfieren entre, el merge se puede realizar automaticamente 
 * si hay confilicros git pedira al usuario que resuelva los conflictos

 Introduccion a shell Script

## introduccion a shell script
- Kenneth lane 1971
primera shell

- William Nelson Jay 1978
shell c

- David Korbn 1983
funciones avanzadas de scripting

- Brian J. Fox 1988
autor orignal del BASH
------------------------------------------------------------------------------------------------------------------------------------------

## Terminologia Shell Script
´Bash´: es un interprete de comandos mas popular - entre el kernel unix y los usuarios.

¨Shell Script¨: permite automotizar procesos y reducir probabilidades de error, son ejecutadas por una shell.

¨Prompt¨: Caracter o un conjunto de caracteres que se muestran en la lista de comandos.

Editor de texto: Permite crear y modificar archivos digitales

--------------------------------------------------------------------
## Iniciando con shell script

------------------------------------------------------------------------------------------------------------------------------------------
## Uso de la Consola o Terminal
Comandos:
history - historial de comandos 
history |grep sudo - todos los comandos que tenga la palabra sudo es un filtro
!54 - ejecuta el comando listado con 54
-----------------------------------------------------------------------------------------------------------------------------------------
comandos de ayuda:
Help - man -f || man -k - info
------------------------------------------------------------------------------------------------------------------------------------------
grep
busqueda de palabras, simbolos, letras numeros y  cualquier patron dentro de un archivo

Sintaxis
grep[opciones]pattern[archivo]
------------------------------------------------------------------------------------------------------------------------------------------
# Alias
Alias Variable="comando_que_Ejecute_la_abreviatura"
## tipos de alias
- Temporal
- Permanente
- Ejemplos
## comandos basicos de archivos o directorios
rm: remueve un archivo
rm dir: Elimina un directorio
rm dir -r: Elimina todo el directorio
mv: mueve un archivo
cp: copia un archivo
cd: cambio entre el directorio
chown: cambio de usuario
chmod:Establecer de permisos a archivos o directorios
tree: 
history: Historial de comandos utilizados anteriormente
## Variables
´´´ bash
echo variable
// output: Valor_de_variable
´´´

## Estructura de Control
### Control de Flujos
- Ejecucion linea a linea o paso por paso
- Bucle(for)
- if(condicional)
- until hasta que se ejcute una condicion
- while mientras
## Uso de Cron y Crontab
son utilizadas para programar una tarea repetitivas en el sistema operativo. Estos elementos permiten establecer tareas programadas para ejecutarse en un momento determinado.
00 19 ** consulta.sh
minutos 0-59 
horas 0-23 
dias 1-31 del mes 
meses 1-12 
dia de la semana 0-6 0 es domingo
