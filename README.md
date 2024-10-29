# **Práctica 1: introducción a Git**

>Este documento tiene como objetivo proporcionar una descripción simple de la implementación y funcionalidad de los comándos básicos de Git.

### Descripción de la práctica

>Se inicializo un nuevo repositorio con el nombre "ProyectoEjemploGit" mediante la herramienta de Git con la cúal repasaremos los comandos y el uso principal y básico de Git y Github.

Para la realización de la práctica vamos a usar como ejemplo el archivo HolaMundo.py mediante el cuál realizaremos varios cambios, los subiremos a nuestro repositorio en diferentes momentos con diferentes mensajes para observar y tener resultados de cómo hacer uso de estas herramientas.

Usaremos un archivo ".gitignore" para mostrar como evitar que archivos que no queramos subir a nuestro repositorio se ignoren, para esto usaremos otro archivo "debug.log" el cual esta solamente de manera local en mi equipo dentro de la misma carpeta en la que se encuentran todos los archivos que se presentan en el presente repositorio.

### Instrucciones de uso

>Para poder hacer uso del archivo HolaMundo.py es necesario descargarlo o copiarlo directamente desde el repositorio.

El archivo se puede ejecutar de dos maneras, ya sea por terminal o con algun IDE para Python.

En cualquiera de los dos casos es necesario tener instalado en nuestro equipo el compilador para python.

En este caso se puede ejecutar directamente desde terminal con la siguiente instrucción ubicandonos en la carpeta que contiene el archivo "HolaMundo.py".

>**python3 HolaMundo.py**

### Comandos utilizados
>En la siguiente tabla se muestran los principales comandos que se usarón para realizar la práctica.

|   Comandos	|   Uso	|
|---	|---	|
| **git --version**	|Se usó para verificar que la instalación de git fuera correta|
| **git init** | Se usó para inicializar el repositorio en el directorio deseado|
| **git config --global user.name** | Se usó para configurar el nombre de usuario en Git |
| **git config --global user.email** | Se usó para configurar el correo que usaremos en Git |
| **git remote add** | Se usó para agregar el servidor remoto al servidor local|
| **git commit -m {comentario}** | Se usó para agregar los cambios al repositorio con un comentario |
| **git push {nombre del servidor} {nombre del branch}**| Se usó para publicar los cambios en nuestro repositorio |
| **git status**| Se usó para ir llevando un seguimiento de los cambios en el índice del repositorio|

### Notas sobre el archivo .gitignore

>El proposito del archivo ".gitignore" es el de llevar un control de los archivos que no queremos que se suban a nuestro repositorio cuando se encuentran en la misma carpeta de manera local (o mejor dicho, no se les dará seguimiento a estos archivos). Para esto dentro del archivo ".gitignore" debemos colocar de manera especifica los archvios que vamos a ignorar, pero como muchas veces pueden ser muchos los archivos y tienen diferentes tipos de archivos, podemos hacer uso de algunos valores que nos permiten seleccionar multiples archivos en una sola línea dentro de éste archivo o hasta rutas especificas que ignorar.

> Para esta práctica se ignora el archivo "debug.log", podemos darnos cuenta que no se le esta dando seguimiento porque:

- Al revisar nuestro archivo ".gitignore" podemos observar con la linea de código que esta dentro del archivo que se ignoran todos los archivos .log.

- Se puede observar que en el repositorio actual no existe el archivo.

- Cuando ejecucatmos en terminal la linea: "**git status**" podemos observar que jamás aparece este archivo en las opciones para ejecutar nuestro commit.