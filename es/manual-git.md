# Manual de Git #

[TOC]

## Introducción

En este manual se hará una introducción breve y concisa del sistema de control de versiones [Git](http://git-scm.com), teniendo en cuenta que para una completa documentación, hay que dirigirse a la [página oficial del manual](http://git-scm.com/documentation).

## Sistemas de control de versiones

Un **sistema de control de versiones** es un software que se usa para llevar un seguimiento de los cambios realizados sobre un archivo o un un conjunto de ellos, además de tener un registro de los mismos y poder volver a cualquier estado anterior.

Generalmente, estos sistemas se utilizan para llevar el seguimiento del código fuente de aplicaciones de software, aunque es posible (y recomendable) utilizarlos para llevar el siguiento de cualquier tipo de información.

Los sistemas de control de versiones comenzaron a desarrollarse y utilizarse cuando los proyectos de software eran demasiado grandes para tener un control de su código y, sobre todo, cuando varios equipos de personas empezaron a trabajar simultáneamente sobre ellos, apareciendo la necesidad de controlar quién cambia qué y de poder volver a versiones anteriores para deshacer cambios con errores.

Algunos sistemas de control de versiones son [RCS (histórico)](http://es.wikipedia.org/wiki/RCS), [CVS (obsoleto)](http://es.wikipedia.org/wiki/CVS), [Subversion](http://es.wikipedia.org/wiki/Subversion), [Mercurial](http://es.wikipedia.org/wiki/Mercurial), [Git](http://es.wikipedia.org/wiki/Git), [etcétera](http://es.wikipedia.org/wiki/Programas_para_control_de_versiones).

### Terminología

Aunque hay muchos sistemas de control de versiones diferentes, la mayoría de ellos comparten la misma terminología. Entre ella se encuentran los siguientes conceptos:

* Repositorio:
* Revisión:
* Rama (*branch*):
* Etiqueta (*tag*):
* Cambio (*changeset*):
* Conflicto:
* *Checkout* (despliegue):
* *Commit* (publicación/envío):
* *Merge* (integración):
* *Update* (actualización):
* Copia de trabajo (*workspace*):

***Nota***: *Cada concepto suele tener asociado otro nombre, bien en inglés o en español. Se suelen usar indistintamente aunque dando prioridad al que está escrito fuera de paréntesis.*

### Tipos

Existen dos tipos de sistemas de control de versiones:

* Centralizados:

* Distribuidos:

## Git

## Configuración

--- git config ---

## Personalización

--- __git_ps1 ---

## Creación de proyectos

--- git init ---
--- git clone --- (view next section)

## Gestión de código

## Flujo de trabajo

Existen varios tipos de flujos de trabajo. Entre ellos están:

* Centralizado:
* Con gestor de integraciones:
* Dictador y tenientes:

El flujo de trabajo que se suele usar con Git es...

## Deshaciendo cosas

### Devolver el repositorio a un estado anterior

--- git reset ---

### Deshacer un *merge* y/o un *rebase* intermedio

Si durante un *merge* o un *rebase* surgen conflictos, Git deja el repositorio en un estado intermedio que obliga al usuario a solucionarlos. Si no se desea darles solución, tanto el *merge* como el *rebase* se pueden deshacer hasta el estado inicial mediante la opción `--abort` de ambos comandos.

## Trabajando en remoto

### Configuración de repositorios remotos

### Añadir referencias remotas

--- git remote add ---

### Clonar, enviar y recibir datos

--- git clone ---
--- git fetch/pull ---
--- git push ---

### Repositorio con varios remotos

--- git remote add ---
--- git fetch/pull *remote* *branch*

### Ramas remotas

## Comandos básicos

## Referencias

[1] [Manual completo Git](http://git-scm.com)
[2] [Git en la Wikipedia](http://es.wikipedia.org/wiki/Git)
