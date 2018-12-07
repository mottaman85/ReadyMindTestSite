# ANGULAR 
## GETTING STARTED

 **Angular** ayuda a construir aplicaciones modernas para la web, el móvil o el escritorio.
Esta guía muestra cómo construir y ejecutar una aplicación Angular simple. Utilizará la herramienta Angular CLI para acelerar el desarrollo, mientras se adhiere a las recomendaciones de la Guía de estilo que benefician a todos los proyectos de Angular.
La guía dura menos de 30 minutos en completarse. Al final, como parte de la revisión final del código, hay un enlace para descargar una copia del código final de la aplicación. (Si no ejecutan los comandos en esta guía, aún puede descargar el código final de la aplicación).

#  REQUISITOS

Antes de comenzar, asegúrese de que su entorno de desarrollo incluya **Node.js®** y un administrador de paquetes npm.

### NODE.JS 

Angular requiere Node.js versión 8.xo 10.x.

 1. Para verificar su versión, ejecute node -v en una ventana de terminal / consola.
 2. Para obtener Node.js, vaya a **nodejs.org**.

### GESTOR DE PAQUETES npm

Las aplicaciones Angular, Angular CLI y Angular dependen de las características y funcionalidades proporcionadas por las bibliotecas que están disponibles como paquetes npm. Para descargar e instalar paquetes npm, debe tener un administrador de paquetes npm.

Este Inicio rápido utiliza la interfaz de línea de comandos del cliente npm, que se instala con **Node.js** de forma predeterminada.

Para verificar que tiene instalado el cliente npm, ejecute npm -v en una ventana de terminal / consola.

## PASO 1: INSTALACIÓN DEL CLI ANGULAR

Se usa la  CLI angular para crear proyectos, generar aplicaciones y códigos de biblioteca, y realizar una variedad de tareas de desarrollo en curso, como pruebas, agrupación e implementación.
Para instalar la CLI usando npm, abra una ventana de terminal / consola e ingrese el siguiente comando: 
**npm install -g @angular/cli**


## PASO 2: CREAR UN ESPACIO DE TRABAJO Y UNA APLICACIÓN INICIAL

Un espacio de trabajo contiene los archivos para uno o más proyectos. Un proyecto es el conjunto de archivos que comprende una aplicación, una biblioteca o pruebas de extremo a extremo (e2e).

Para crear un nuevo espacio de trabajo y un proyecto de aplicación inicial:

Ejecute el comando CLI ng new y proporcione el nombre my-app, como se muestra aquí:
**ng new my-app**

El nuevo comando **ng** solicita información sobre las características que debe incluir en el proyecto de aplicación inicial. Acepte los valores predeterminados presionando la tecla Intro o Retorno.
Angular CLI instala los paquetes Angular **npm** necesarios y otras dependencias. Esto puede tardar unos minutos.

También crea los siguientes archivos de proyecto de área de trabajo y de inicio:

 - Un nuevo espacio de trabajo, con una carpeta raíz llamada my-app
 - Un proyecto inicial de la aplicación de esqueleto, también llamado my-app 	  (en la subcarpeta src)
 - Un proyecto de prueba de extremo a extremo (en la subcarpeta e2e)
 - Archivos de configuración relacionados

El proyecto de aplicación inicial contiene una aplicación de bienvenida, lista para ejecutarse.

## PASO 3: EJERCER LA APLICACIÓN

Angular incluye un servidor, de modo que puede construir y ejecutar su aplicación fácilmente de manera local.  

 1. Vaya a la carpeta del área de trabajo (my-app).     
 2. Inicie el servidor utilizando el comando CLI ng serve, con la opción --open.

El comando ng serve inicia el servidor, observa sus archivos y reconstruye la aplicación a medida que realiza cambios en esos archivos.
La opción --open (o simplemente -o) abre automáticamente su navegador en http: // localhost: 4200 /.
La aplicación inicia en la web con un *saludo* 

## PASO 4: EDITAR TU PRIMER COMPONENTE EN ANGULAR

los componentes son fundamentales de las aplicaciones Angular. Muestran datos en la pantalla y toman medidas en función de esa entrada.
Como parte de la aplicación inicial, la CLI creó el primer componente angular. Es el componente raíz, y se llama app-root.

 1. Abrir ./src/app/app.component.ts.
 2. Cambie la propiedad del título de 'my-app' a **'My First Angular App'**.

Código:

@[Component](https://angular.io/api/core/Component)({ selector:  'app-root', 
																								templateUrl: './app.component.html',  
																								[styleUrls](https://angular.io/api/core/Component#styleUrls):  [ './app.component.css']  })  
																								export  class  AppComponent  { 
																								title =  'My First Angular App!';  }

El navegador se actualiza automáticamente con el título revisado.

3. Abrir ./src/app/app.component.css y dar estilo al component.css.

h1 { color:  #369; 
font-family:  Arial,  Helvetica, sans-serif; 
font-size:  250%;  }

Al final aparecerán los cambios efectuados en el navegador. 
