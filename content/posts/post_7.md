---
title: "Comandos basicos"
date: 2022-05-24
description: 'Comandos basico para usar linux'
---

#Bienvenido

Todo sistema operativo contiene un CLI que significado es interfaz linea de comando por sus siglas en ingles, pero linux tiene su uso más en linea de comandos, que otros como windows y mac tiene mas interfaz graficas. que es la razón por la que linux es mas en servidores mientras que los otros sistemas apuestan más a la interfaz grafia de usuario, pero tampoco es pensar que solo es para usuarios avanzados, cualquier persona puede usarlo solo es quitarse el miedo, aunque puede ir realizando pruebas montando una maquina virtual.

los siguientes comando te ayudaran a familiarizarse con el sistema operativo linux.
**Usaremos estos comandos para Distro Ubuntu, tambien puedes aplicarlos en otros**

* Conocer donde estamos ubicados

```
pwd

```
Ejemplo: 
- soylinux@linux:~$ pwd 
- /home/soylinux

* para navegar entre directorios

```
- cd [Nombre de la carpeta o puede agregara la ruta donde quiere ir]
- cd ..  [ tambien puede agregara la ruta donde quiere ir, despues de los puntos]
```
Ejemplo: 
para ir asi adelante 
- soylinux@linux:~$ cd /home
- soylinux@linux:/home~$ 

para regresa 
- soylinux@linux:~$ cd /home
- soylinux@linux:/home~$ cd ..
- soylinux@linux:~$


* crear una carpeta 

```
mkdir
mkdir [Nombre de la carpeta]

```
Ejemplo: 
- soylinux@linux:~$ mdkir example

* ver lo que contiene nuestra carpeta

```
ls 
ls -l

```
Ejemplo: 

- soylinux@linux:/home~$ ls
- soylinux
- soylinux@linux:/home~$ ls -l
- drwxr-xr-x 42 soylinux soylinux 4096 sep 30 16:42 soylinux
