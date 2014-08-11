# Manual de Git #

[TOC]

## Introducción

En este manual se hará una introducción breve y concisa del sistema de control de versiones [Git](http://git-scm.com), teniendo en cuenta que para una completa documentación, hay que dirigirse a la [página oficial del manual](http://git-scm.com/documentation).

## Sistemas de control de versiones

Un **sistema de control de versiones** es un software que se usa para llevar un seguimiento de los cambios realizados sobre un archivo o un un conjunto de ellos, además de tener un registro de dichos cambios y poder volver a cualquier estado anterior.

Generalmente, estos sistemas se utilizan para llevar el seguimiento del código fuente de aplicaciones de software, aunque es posible utilizarlos para llevar el siguiento de cualquier tipo de información.

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

Existe un repositorio maestro donde todos los usuarios acceden tanto para hacer hacer *checkout* como para hacer *commit*. Un ejemplo de sistema de control de versiones centralizado es Subversion.

* Distribuidos:

No existe un repositorio maestro. Cada usuario tiene una copia completa del repositorio y hace las modificaciones que considera oportunas. Una vez hechas, realiza la que se llama un *pull request* para indicar a otro usuario que el primero quiere incorporar sus cambios en el segundo.

Un repositorio distribuido también puede funcionar como repositorio centralizdo siempre que todos los usuarios tengan conocimiento de este.

## Git

Git es un sistema de control de versiones distribuido creado por Linus Torvalds en 2005. Todo el proyecto y toda la información asociada a él están en la máquina del desarrollador, por lo que no es necesario ningún repositorio central. Cuando dicho desarrollador quiere incluir sus cambios en el repositorio de otro desarrollador, este inicia un *pull request* (que puede ser realizdo de varias formas).

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

## Lista completa de comandos

* `git`: Comando principal (llama al resto).
* `git-add`: Añade archivos al respositorio para hacer seguimiento o indica que un archivo tiene cambios para hacer un *commit*.
* `git-add--interactive`: Forma interactiva de `git add`.
* `git-am`: Aplica parches recibidos por correo electrónico.
* `git-annotate`: Sinónimo de `git blame`.
* `git-apply`: Aplica parches a archivos y/o al índice.
* `git-archimport`: Importa repositorios de Arch Linux.
* `git-archive`: Exporta archivos de un repositorio.
* `git-bisect`: Ayuda a encontrar el cambio que introdujo un error.
* `git-bisect--helper`: 
* `git-blame`: Indica el autor de cada modificación en cada línea.
* `git-branch`: Crea una rama nueva.
* `git-bundle`: Crea un archivo para enviar objectos y referencias entre repositorios.
* `git-cat-file`: Muestra información de objectos del repositorio.
* `git-check-attr`: Chequea attributos de Git (del archivo `.gitattributes`).
* `git-check-ignore`: 
* `git-check-mailmap`: 
* `git-checkout`: Obtiene una rama o unos archivos copiándola en la copia de trabajo.
* `git-checkout-index`: Obtiene archivos del índice copiándolos a la copia de trabajo.
* `git-check-ref-format`: 
* `git-cherry`: 
* `git-cherry-pick`: 
* `git-citool`: Herramienta gráfica para hacer *commit*.
* `git-clean`: Elimina todos los archivos que no están bajo el control de versiones.
* `git-clone`: Clona un repositorio en un directorio nuevo.
* `git-column`: 
* `git-commit`: 
* `git-commit-tree`: 
* `git-config`: 
* `git-count-objects`: 
* `git-credential`: 
* `git-credential-cache`: 
* `git-credential-cache--daemon`: 
* `git-credential-store`: 
* `git-cvsexportcommit`: 
* `git-cvsimport`: 
* `git-cvsserver`: 
* `git-daemon`: 
* `git-describe`: 
* `git-diff`: 
* `git-diff-files`: 
* `git-diff-index`: 
* `git-difftool`: 
* `git-difftool--helper`: 
* `git-diff-tree`: 
* `git-fast-export`: 
* `git-fast-import`: 
* `git-fetch`: 
* `git-fetch-pack`: 
* `git-filter-branch`: 
* `git-fmt-merge-msg`: 
* `git-for-each-ref`: 
* `git-format-patch`: 
* `git-fsck`: 
* `git-fsck-objects`: 
* `git-gc`: 
* `git-get-tar-commit-id`: 
* `git-grep`: 
* `git-gui`: 
* `git-gui--askpass`: 
* `git-hash-object`: 
* `git-help`: 
* `git-http-backend`: 
* `git-http-fetch`: 
* `git-http-push`: 
* `git-imap-send`: 
* `git-index-pack`: 
* `git-init`: 
* `git-init-db`: 
* `git-instaweb`: 
* `git-log`: 
* `git-ls-files`: 
* `git-ls-remote`: 
* `git-ls-tree`: 
* `git-mailinfo`: 
* `git-mailsplit`: 
* `git-merge`: 
* `git-merge-base`: 
* `git-merge-file`: 
* `git-merge-index`: 
* `git-merge-octopus`: 
* `git-merge-one-file`: 
* `git-merge-ours`: 
* `git-merge-recursive`: 
* `git-merge-resolve`: 
* `git-merge-subtree`: 
* `git-mergetool`: 
* `git-mergetool--lib`: 
* `git-merge-tree`: 
* `git-mktag`: 
* `git-mktree`: 
* `git-mv`: 
* `git-name-rev`: 
* `git-notes`: 
* `git-p4`: 
* `git-pack-objects`: 
* `git-pack-redundant`: 
* `git-pack-refs`: 
* `git-parse-remote`: 
* `git-patch-id`: 
* `git-prune`: 
* `git-prune-packed`: 
* `git-pull`: 
* `git-push`: 
* `git-quiltimport`: 
* `git-read-tree`: 
* `git-rebase`: 
* `git-rebase--am`: 
* `git-rebase--interactive`: 
* `git-rebase--merge`: 
* `git-receive-pack`: 
* `git-reflog`: 
* `git-relink`: 
* `git-remote`: 
* `git-remote-ext`: 
* `git-remote-fd`: 
* `git-remote-ftp`: 
* `git-remote-ftps`: 
* `git-remote-http`: 
* `git-remote-https`: 
* `git-remote-testsvn`: 
* `git-repack`: 
* `git-replace`: 
* `git-request-pull`: 
* `git-rerere`: 
* `git-reset`: 
* `git-revert`: 
* `git-rev-list`: 
* `git-rev-parse`: 
* `git-rm`: 
* `git-send-email`: 
* `git-send-pack`: 
* `git-shell`: 
* `git-sh-i18n`: 
* `git-sh-i18n--envsubst`: 
* `git-shortlog`: 
* `git-show`: 
* `git-show-branch`: 
* `git-show-index`: 
* `git-show-ref`: 
* `git-sh-setup`: 
* `git-stage`: 
* `git-stash`: 
* `git-status`: 
* `git-stripspace`: 
* `git-submodule`: 
* `git-svn`: 
* `git-symbolic-ref`: 
* `git-tag`: 
* `git-unpack-file`: 
* `git-unpack-objects`: 
* `git-update-index`: 
* `git-update-ref`: 
* `git-update-server-info`: 
* `git-upload-archive`: 
* `git-upload-pack`: 
* `git-var`: 
* `git-verify-pack`: 
* `git-verify-tag`: 
* `git-web--browse`: 
* `git-whatchanged`: 
* `git-write-tree`: 

## Referencias

[1] [Manual completo Git](http://git-scm.com)
[2] [Git en la Wikipedia](http://es.wikipedia.org/wiki/Git)
