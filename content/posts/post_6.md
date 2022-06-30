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



para empezar a usar Git no estan tan complicado, por lo que te mostrare los comando básicos. 

-Abrir su terminal favorita.

Crear una carpeta, será el principal que se ejecutara el git para que reconozca todo dentro. 

Ejecutamos el siguiente comando

> mkdir mi-proyecto


para versionar el proyecto ejecutamos el comando siguiente comando. 

> Git init

este crea un subdirectorio con sus componentes necesarios denominado .git y lo mantiene oculto


> Git status

nos va ayudar a conocer los archivos que estara versionando Git, y así mismo poder indicarle los archivos necesarios versionar.


> Git add hola.txt
> Git add * 
