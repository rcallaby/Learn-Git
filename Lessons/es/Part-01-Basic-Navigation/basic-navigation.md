# Git - Navegación Básica

- [Introducción](#introducción)
- [Abrir la Terminal BASH](#abrir-la-terminal-bash)
- [Navegar a través de Directorios](#navegar-a-través-de-directorios)
- [Listar Contenidos de Directorios](#listar-contenidos-de-directorios)
- [Crear y Mover Directorios](#crear-y-mover-directorios)
- [Crear y Eliminar Archivos](#crear-y-eliminar-archivos)
- [Conclusión](#conclusión)

# Introducción:
La terminal BASH es una interfaz de línea de comandos poderosa que permite a los usuarios navegar por el sistema de archivos de su computadora, realizar diversas tareas e interactuar con sistemas de control de versiones como Git. Git es un sistema de control de versiones distribuido ampliamente utilizado que proporciona colaboración eficiente y seguimiento de cambios en repositorios de código. En este artículo, exploraremos cómo navegar y utilizar comandos básicos en la terminal BASH para trabajar eficazmente con Git.

## Abrir la Terminal BASH:
Para comenzar, abre tu aplicación de terminal preferida. En la mayoría de los sistemas basados en Unix, puedes encontrar la terminal en la carpeta "Aplicaciones" o "Utilidades". Una vez lanzada, aparecerá un símbolo del sistema listo para aceptar tus comandos.

## Navegar a través de Directorios:

El comando `pwd` significa "Print Working Directory" y muestra la ruta del directorio de trabajo.
```commandline
pwd
```
Este comando no tiene argumentos u opciones.

El comando `cd` (abreviatura de "change directory") es fundamental para navegar por el sistema de archivos. Aquí tienes algunos ejemplos comunes de uso de `cd`:

Para moverte a un directorio, usa `cd <directorio>` (sustituye `<directorio>` por el nombre del directorio deseado), como por ejemplo:
```
cd Documentos
```
Para retroceder un nivel de directorio, escribe `cd ..` como por ejemplo:
```
cd ..
```
Para ir a tu directorio de inicio, usa `cd` o `cd ~` como por ejemplo:
```
cd ~
```
Para moverte al directorio anterior, usa `cd -` como por ejemplo:
```
cd -
```

## Listar Contenidos de Directorios:
El comando `ls` se utiliza para listar el contenido de un directorio. De forma predeterminada, muestra los archivos y directorios en el directorio actual. Algunas banderas útiles para mejorar la funcionalidad de `ls`:

`ls -l` muestra el contenido en un formato de lista detallada.
```commandline
ls -l
```
`ls -a` muestra archivos y directorios ocultos.
```commandline
ls -a
```
`ls -h` proporciona tamaños de archivo legibles por humanos.
```commandline
ls -h
```
`ls -R` lista directorios y sus contenidos de forma recursiva.
```commandline
ls -R
```

## Crear y Mover Directorios:
Puedes crear directorios usando el comando `mkdir` seguido del nombre del directorio deseado:
Para crear un directorio en la ubicación actual, usa `mkdir <directorio>`. Por ejemplo:
```
mkdir estedirectorio
```
Para crear directorios anidados, utiliza `mkdir -p <directorio_padre>/<directorio_hijo>`.
```
mkdir -p estedirectorio/subdirectorio
```
Para eliminar directorios, utiliza el comando `rmdir`:
`rmdir <directorio>` elimina un directorio vacío.
```commandline
rmdir estedirectorio
```

Mover y Renombrar Archivos y Directorios:
El comando `mv` te permite mover y renombrar archivos y directorios:
Para mover un archivo o directorio, utiliza `mv <origen> <destino>`. Por ejemplo:
```commandline
mv estedirectorio nuevonombredirectorio
```

Para renombrar un archivo o directorio, utiliza `mv <nombre_antiguo> <nombre_nuevo>`.
```commandline
mv viejodirectorio nuevodirectorio
```

## Crear y Eliminar Archivos:
Puedes crear un nuevo archivo usando el comando `touch`.
```commandline
touch nuevo_nombre_de_archivo
```
O en un directorio, como por ejemplo:
```commandline
touch directorio/nuevo_nombre_de_archivo
```
Ahora, eliminemos un archivo usando el comando `rm`.
```commandline
rm nombre_de_archivo
```
Para eliminar directorios y sus contenidos de forma recursiva
```commandline
rm -r nombre_de_archivo
```
Para ignorar archivos y argumentos que no existen, sin preguntar nunca.
```commandline
rm -f nombre_de_archivo
```
Para verificar lo que se está haciendo
```commandline
rm -v nombre_de_archivo
```
Para eliminar todo dentro de un directorio.
```commandline
rm *
```
# Conclusión:
La terminal BASH, junto con Git, ofrece un entorno sólido para un control de versiones eficiente y una gestión de archivos efectiva. Al familiarizarte con comandos básicos como `mkdir`, `rmdir`, `rm`, `mv`, `cd`, `ls`, `pwd` y comandos específicos de Git como `git init`, `git add`, `git commit`, `git push` y `git pull`, puedes navegar por directorios, crear y eliminar directorios, mover y renombrar archivos, eliminar archivos y gestionar eficazmente tus repositorios de Git. La práctica y la exploración te ayudarán a volverte más competente en el uso de estos comandos, permitiéndote optimizar tu flujo de trabajo de desarrollo.
```