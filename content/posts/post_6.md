---
title: "Uso del GIT"
date: 2022-05-24
description: 'Comandos basico para usar GIT'
---

# Antes de seguir con la lectura...

*Hola visitante*

Quisiera mencionar Git y github lo confunden mucho, pero la realidad es que ambos son distintos. 

- Git es un sistema de control de versiones, esta Diseñado para manejar desde grandes a pequeños proyectos y es un free and open source. 
- GitHub es una plataforma  de desarrollo colaborativo, permitiendo alojar proyectos utilizando el sistema de control de version el Git,


Ultimamente conforme he estado investigando tanto viendo tutoriales, libros y por medio del internet, cuando se empieza a realizar un proyecto lo primordial a saber es el Git, este sistema nos facilita mucho el trabajo, imaginate empezar un proyecto llamado 'mi-primer-proyeco' luego conforme vayamos haciendo cambios no queremos dañar el original, por lo que optamos por crear una copiar, así sucesivamente hasta tener un varios por motivo de cambios, con este sistemas podremos evitar crear miles de copias del primer proyecto llamandoles de distintos nombres e igual nos ayudaria a la colaboración y trabajo en equipo.

para usar el git tienes que tener instalado [Guía de Instalación](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 
 
puedes visualizar la version con el siguiente comando

>git --version


para empezar a usar Git no estan tan complicado, por lo que te mostraré los comando básicos. 

- Abrir su terminal favorita.
- Configuramos Git, Primero tenemos que definir algunas variables globales el user.name y user.email, ambas son necesarias para las confirmaciones 

Establecemos un nombre con el siguiente comando, remplazando el <USER_NAME> por un nombre que se desea usar.

> git config --global user.name "<USER_NAME>"

ahora establecemos un corre con el siguiente comando,remplazando el <USER_EMAIL> por su dirección de correo electrónico .
> git config --global user.email "<USER_EMAIL>"

ahora para validar la información usamos el siguiente comando 

> git config --list 

obteniendo una salida de información como el ejemplo 

user.name=Diegohc
user.email=soygit@correo.com

## Es momento de crear un directorio proyecto

Crear una carpeta, será el principal que se ejecutara el git para que reconozca todo dentro. 

Ejecutamos el siguiente comando

> mkdir mi-proyecto

accedemos a la carpeta

cd mi-proyecto

para versionar el proyecto ejecutamos el siguiente comando. para la versione 2.28.0 o superior se aplica un distinto comando que ayuda facilitar el inicio y la creación de la rama main, pueden ser dos comando diferentes:

> git init --initial-branch=main
> 
> git init -b main

para versiones anterios el tradicional. 

> git init

creación de la rama main y el cambio.
> git checkout -b main

este crea un subdirectorio con sus componentes necesarios denominado .git y lo mantiene oculto


> git status

nos va ayudar a conocer los archivos que estara versionando Git, y así mismo poder seleccionar los archivos necesarios versionar.


> git ignore *.doc

antes de indicarle a git que archivos versionar, debemos tener encuenta que hay archivos no es necesario versionar, ya que por lo generar son llamados archivos temporales, es decir que pueden volver a crear cada vez que se ejecuta un comando. primero tienes que crear un archivo - .gitignore- tene que estar en la carpeta principal del proyecto, con este comando podemos indicarle a git que no queremos 
que esos archivos sean versionados. sin embargo hay un reposistorio que puede ayudarte a ver que archivos pueden ser agregados al archivo ignore - link del [gitignore](https://github.com/github/gitignore) 



> git add hola.txt
> 
> git add * 

una vez visualizado los archivos que el git reconoce para versionar. ahora toca indicarle a git que archivos se van a versionar, por lo que hay dos maneras, la primera es indicandole mediante el comando add  seguido del nombre del archivo y su extesión como se muestra anteriormente y la segunda es indicarle que todos los archivos que se encuentren en la caperta principal y subcarpetas sin importar la extensión del archivo. puede volver aplicar el comando git status.

> git commit -m "first commit" 

ya agregamos los archivos que se versionaran,  este comando es una de las funciones esenciales principales de Git, este nos permitara realizar la confirmación de los
procesos y los cambios conforme vayamos trabajando en el proyecto, no ayudara crear un punto de restauracion por si en el proceso se comete un error o realizar un cambio. los siguiente son las lletras que usan durante un commit
 > * A - Archivos añadidos al escenario
 > *  M - Archivos modificados
 > *  D - Archivos eliminados

> git log

permite visualizar los commit que se tienen hecho y en la rama. no ayudaria a visualizar los puntos de restauración del proyecto.

> git help

Permite visualizar la informacion de todo los comandos, en caso que se olvide un comando y este puede ayudarlo a recordar, así como igual puede tener de un solo comando usando el siguiente : 

> git <command> --help
