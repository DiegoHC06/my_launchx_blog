---
title: "Proyecto JS"
date: 2022-05-24
description: 'Crear un proyecto de JS'
---
 
 Hola visitante
 
 en este post aprenderemos a crear un proyecto con javaScript
 
 Para la creacion del proyecto utilizaremos Node.js
 
 Es un entorno de tiempo de ejecución JavaScript de código abierto y multiplataforma. 
 ¡Es una herramienta popular para casi cualquier tipo de proyecto!
 
 para eso tenemos que descargar e instalar el Node.js en nuestro equipo. 
 
 [Descargar Nodejs](https://nodejs.dev/download "DescargarNodejs")
 
-----------

##  Creacion de carpeta 
 
Crear una carptea para tu proyecto, puedes nombrarlo a tu gusto y otras dos, una llamada app y la otra test



##  Inicializar el proyecto

Una vez creada la carpeta dentro de ella vamos a inicializar el proyecto con node.js utilizando el siguiente comando

>   npm init

Este nos va crear un arhivo llamada Package.js conforme a la instalacion nos pedira un datos a llenar o bien darle solo
enter y luego se puede rellenar los datos, a continuación un ejemplo. ESte archivo sera el corazón del proyecto.

```javascript
{
  "name": "miapp",
  "version": "1.0.0",
  "description": "Proyecto para mi crear mi primera app ",
  "main": "index.js",
  "scripts": {
    "test": "node ./node_modules/.bin/jest" 
  },
  "author": "Diego ",
  "license": "ISC",
  "devDependencies": {
    "jest": "^28.1.0"
  }
}

```
como recordatorio la ruta del test es distinto dependiendo del sistema operativo.

## Instalación de Dependencias.

Para instalar las dependencias, es posicionarse siempre en la carpeta del proyecto se ejecuta el siguiente comando

>   npm install  -La dependencia-

verificar en el proyecto que creo un carpeta llamada node_modules, **Importante no versionarlo**, para no versiona dicha carpeta se tiene que crear 
un archivo .gitignore y agregar la linea de **/node_modules dentro del archivo.

        

##  Estructura del proyecto

miapp-
      -node_modules
      -app
      -test
      -package-lock.json
      -package.js
 
- Carpeta app - aqui iran el codigo que se pondra a prueba

- Carpeta test - iran las pruebas para comprabor si esta bien el codigo. 


##  Pruebas de unidad

en la caperta llamada app,  crearemos un archivo llamada app.js. Crear una clase llamada miapp junto con un constructor que recibira unos paremetro,
en este caso solo name, por ultimo no olvidar exportar la clase, acontinuacion una ejemplo.

```javascript
class miapp {
  constructor (name) {
    this.name = name
  }
}

module.exports = miapp
```

en la carpeta test, crear un archivo llamado miapp.test.js, acontinuacion un ejemplo.

```javascript
describe("Esto es una suite de pruebas", () => {
  test('Caso de prueba 1', () => {
    const result = 1 + 2 
    expect(result).toBe(10);
  });
})
```
una vez creado el archivo procedemos a ejecutar el siguiente comando con el archivo

>  npm test  test/missionCommander.test.js

listo, hemos creado un proyecto con javaScript

![image](https://user-images.githubusercontent.com/50012419/170173496-9ef80524-a72a-4a50-9fb8-32b242cabc77.png)


*Si quieres trabajar con node js. te conviene hacer caso a las advertencias 

*Como siempre nos dijo el missionCommander [@carlogilmar ](https://github.com/carlogilmar)

**NO CONFÍES EN UNA PRUEBA QUE NO HAS VISTO FALLAR.**


### Referencias

- https://jestjs.io/
- https://nodejs.org/en/docs/

