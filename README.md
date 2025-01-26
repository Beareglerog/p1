# Memoria de la Práctica 1

### Enlaces a ficheros usados

[PDF explicación comandos](git.pdf)
[PDF requisitos de entorno](entorno.pdf)

## Comandos

#### git clone:

_git clone https://github.com/gitt-3-pat/p1_

Este comando se usa para copiar un repositorio remoto a tu equipo local. En este caso lo he usado para copiar el repositorio de práctica 1 aportado por el profesor, a mi entorno local.

**Log tras la ejecución:**

Cloning into 'p1'...
remote: Enumerating objects: 15, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 15 (delta 1), reused 15 (delta 1), pack-reused 0
Receiving objects: 100% (15/15), done.
Resolving deltas: 100% (1/1), done.

En este caso lo he usado para comprobar si existían archivos por confirmar o agregar en mi repositorio local o algún archivo modificado

## git status:

Este comando muestra el estado actual del repositorio local. Permite ver los cambios realizados y el estado de los archivos. Como se acaba de mencionar, lo he usado para ver si existían archivos por confirmar o agregar en mi repositorio local. 

**Log tras la ejecución:**

On branch main
Your branch is up to date with 'origin/main'.
Untracked files:
(use "git add <file>..." to include in what will be committed)
p1/
nothing added to commit but untracked files present (use "git add" to track)

En este caso lo he usado para comprobar si existían archivos por confirmar o agregar en mi repositorio local o algún archivo modificado.

## git add:

**git add .**

Este comando preparar los archivos que se han creado o modificado para ser confirmados (commit) en el repositorio de Git

## git commit:

_git commit -m "TU MENSAJE"_

Este comando confirma los cambios que se han añadido y los guarda en el historial del repositorio local.

**Log tras la ejecución:**

[main f403ffb] TU MENSAJE
 1 file changed, 1 insertion(+)
 create mode 160000 p1

 Como se ha mencionado, he usado commit para guardar los cambios realizados en el archivo “.”. Cabe mencionar que debería haber cambiado el mensaje a “Añadido correctamente” o algo del estilo

## git push:

Este comando coge los cambios que se han confirmado localmente (commit) y los sube al repositorio remoto en la rama especificada

**Log tras la ejecucion:**

Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 265 bytes | 265.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Bearglerog/p1
   07720b5..f403ffb  main -> main

*Nos ha indicado que se ha subido a main correctamente

A continuación, he usado este comando para subir el archivo y otros cambios confirmados al repositorio remoto en la rama principal main.

## git checkout 

_git checkout -b feature/1_
_git checkout main_

Este comando se utiliza para cambiar entre ramas

**Log tras la ejecucion:**

Switched to branch 'main'
Your branch is up to date with 'origin/main'.
*Confirma que la rama main está sincronizada con la rama remota origin y que no hay cambios pendientes.

