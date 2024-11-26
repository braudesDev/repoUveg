## Leccion 1. Introducción a las aplicaciones móviles hibridas.

- Para la construcción del contenido en la aplicación móvil hacen uso de HTML, PUG, etc.

- Para definir los estilos de los elementos gráficos hacen uso de CSS, SCSS, SASS, etc.

- Para la lógica de programación hacen uso de JavaScript, TypeScript, etc.

Que es un Framework?
Un framework facilita el trabajo en equipo, ya que cuando todos los integrantes conocen los estándares del framework es más fácil para los compañeros identificar las secciones en las cuales se va a trabajar o a realizar alguna modificación.

## Leccion 2. TypeScript.
### Transpilar. 

En un lado vemos cómo sería con JavaScript, donde solo definimos la variable y asignamos un valor.  
Del otro lado planteamos el mismo ejemplo, pero haciendo uso de TypeScript, donde pueden observar que se escribe el tipo de variable  

var, let, const seguido del nombre de la variable, posteriormente dos puntos y el tipo de dato de la variable. En este caso, lo definimos como String porque es una cadena de texto y lo igualaremos a un valor.

``` JavaScript
_JavaScript_

let name = 'Braulio';  

ó

let name;

name = 'Braulio';

```

``` TypeScript
_TypeScript_

let name: string = 'Braulio';

ó

let name: string;

name = 'Braulio';
```


### Definición de variables en TypeScript.

Primeramente debemos tener instalado  ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) , el gestor de paquetes de NPM y un editor de código como por ejemplo  ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) .  Después solo haría falta instalar el paquete de  ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) . 

#### Instalar en local.

En esta sección copiamos el comando que debemos ejecutar en la terminal (Mac, Linux) o cmd (Windows).

Para instalar  ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) vía npm:

``` bash
npm install -g typescript

```

Ajustar compilaciones a través de tsc:

```bash
npx tsc 
```

Una vez que se ejecuto el comando, mostrara un resumen de lo instalado:

[![resume-Instal-Npm.png](https://i.postimg.cc/g2MCHz9z/resume-Instal-Npm.png)](https://postimg.cc/mPHpbG2J) 
Se abrió  ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) y se ejecuto un mensaje que dijera:

```TypeScript
console.log('Hola mundo!');
```
 Y después de abrió una nueva terminal en ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) para mostrar el mensaje por consola aunque de igual manera podemos usar la consola de nuestro sistema operativo. Pero antes de eso debemos transpilar el código de ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) a ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E).  
 Para transpilar el código se debe ejecutar el siguiente comando en consola:
```bash
tsc HolaMundo.ts
```

Después de eso podemos observar que se nos genera un nuevo archivo pero ahora con la extensión **.js**.  

Ahora, si quisiéramos usar el código ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) en el navegador no funcionaria, por ello es necesario **transpilar** a ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E). Para comprobar el **log**, tan solo ejecutamos el comando **node** seguido del nombre del archivo, en este caso "**node** HolaMundo.js".

**Vista desde la terminal de**  ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  **:** 

```bash
~/Documentos/typeScript$ tsc HolaMundo.ts
~/Documentos/typeScript$ node HolaMundo.js
Hola mundo!
```


[![muestra-Por-Consola.png](https://i.postimg.cc/qv0y7Vj4/muestra-Por-Consola.png)](https://postimg.cc/QH4H6z2y) 
**Vista desde la terminal de** ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) **:** 

[![muestra-Por-Consola-VSCode.png](https://i.postimg.cc/BQ5Pk7sy/muestra-Por-Consola-VSCode.png)](https://postimg.cc/560tF3Xq)
#### Hacer comentarios en TypeScript

La documentación de un programa es muy importante por ello es que se hagan comentarios para que nos ayude a recordar lo que estábamos haciendo, incluso si alguien mas lee nuestro código, le facilitamos la comprensión.

Forma de comentar en  ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) :

```TypeScript
// Comentario en unsa sola linea

//*
*Comentario multilinea
*/
```

#### Definir variables.
Para definir una variable debemos escribir el tipo de variable **(var, let o const)** seguido del nombre y finalizamos con punto y coma **(;)**.
Si posicionamos el puntero del mouse sobre la variable, nos mostrara que la variable es de tipo **any**, pues no definimos si era una cadena de  **texto, numero, booleano, etc**.

```TypeScript
let firstName;
```

[![definir-Variable.png](https://i.postimg.cc/yY78g14Q/definir-Variable.png)](https://postimg.cc/bdFh4jvk)
Ahora si le podemos asignar una cadena vacía y el editor automáticamente detectara que es un  **string**.

```TypeScript
let firstName = '';
```

[![definir-Variable-Correcto.png](https://i.postimg.cc/FsZx6ZhG/definir-Variable-Correcto.png)](https://postimg.cc/8j7WJLJr)
Si se crea una variable y se le asigna un 0 (cero) sera un tipo de dato numérico:

```TypeScript
let firstName = '';
let age = 0;
```

No es necesario asignar valor a una variable para que tome el tipo de dato, se puede asignar el tipo de dato a una variable cuando es definida.
La forma de hacerlo es la siguiente:

```TypeScript
let firstName = '';
let age = 0;

let isMan: boolean;
```

Después del nombre de la variable se ponen dos puntos **(;)** seguidos del tipo de variable.

**Ventajas de definir un tipo de dato en una variable**:
El editor puede marcar un error donde menciona que no puedes asignar ese valor, puesto que no corresponde al tipo de dato.

```TypeScript
let firstName = '';
let age = 0;

let isMan: boolean = 'false';
```

[![no-Corresponde-Al-Tipo-De-Dato.png](https://i.postimg.cc/vHHn4ddL/no-Corresponde-Al-Tipo-De-Dato.png)](https://postimg.cc/qgSqFSqz)

// Quedan pendientes cosas de la leccion 2 de TypeScript

## Lección 3. Introducción a Angular.

La primera versión que se lanzó de ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) fue en 2010, esta versión hace uso de ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) , de ahí el nombre de ![Angular.js](https://img.shields.io/badge/angular.js-%23E23237.svg?style=for-the-badge&logo=angularjs&logoColor=white) ; si bien actualmente se sigue utilizando, tiene más potencial **Angular 2+** ya que utiliza tecnologías más nuevas como ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) , entre otras.
![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white)  es un *framework* desarrollado por ![Google](https://img.shields.io/badge/google-4285F4?style=for-the-badge&logo=google&logoColor=white). 
**SPA**: *Single Page Application*.
Es Una aplicación web que maneja solamente una única pagina web para mostrar los elementos ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)  Ejemplos de estas paginas son ![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)  y ![Netflix](https://img.shields.io/badge/Netflix-E50914?style=for-the-badge&logo=netflix&logoColor=white) .
![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) es un framework que utiliza el patrón MVC: Modelo Vista Controlador, llamado así por la separación del código en tres capas, las cuales son:

**Modelo:** Es la capa donde se trabaja con los datos.
**Vista:** Es la capa donde se trabaja con la interfaz que va a mostrar al usuario.
**Controlador:** Es la capa donde se ejecutan las acciones que realiza un usuario sobre la aplicación. 

![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white)  hace uso del lenguaje de programación ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)  

Ejemplo de componente:
Las partes se;aladas son un ejemplo de componentes.

[![componentes.png](https://i.postimg.cc/zG9vqsjj/componentes.png)](https://postimg.cc/gxHmDB1X)
**En resumen un componente puede ser desde un botón *input* hasta una pagina completa.**

Un buen proyecto no solo se evalúa por su funcionamiento, lineas de código, etc. También se evalúa por su orden.
Entonces cuando se dice que ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white)  es modular se refiere a que se pueden crear módulos para tener todo mas organizado.

[![grafico.png](https://i.postimg.cc/bYMKVqN3/grafico.png)](https://postimg.cc/8sRKjQv6)
Para poder crear un primer componente vamos a necesitar crear un proyecto con ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) .
Necesitamos: 
Tener instalado ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) y el gestor de paquetes **NPM**. Ademas de instalar el paquete **Angular-cli**. Para ello debemos abrir la terminal y ejecutar el siguiente comando:

```bash
sudo npm install -g @Angular/cli
```

![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white)  cli nos ayuda a generar un proyecto de ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) , cli significa Command Line Interface, es español: Interfaz de Línea de Comandos. 

Una vez instalado el cli de ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white), para crear un proyecto ejecutamos el siguiente comando:
```bash
ng new nombreDelProyecto
```

El mismo sistema nos preguntara si deseamos agregar el ruteo de ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white), solo debemos indicar que si (y).
Enseguida nos pedirá seleccionar el lenguaje de hoja de estilos que deseamos utilizar, en este caso usaremos SCSS.
Finalmente comenzara a crear la estructura del proyecto y a instalar los paquetes necesarios.

[![creacion-Estructura-De-Proyecto.png](https://i.postimg.cc/x1Fx8RJg/creacion-Estructura-De-Proyecto.png)](https://postimg.cc/w1LcbDks)
Para abrir una carpeta en ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)  desde la terminal se debe usar el siguiente comando:

```bash
code ruta/a/la/carpeta 
```

Una vez abierta la carpeta en ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white), nos mostrara algunos directorios, por ejemplo, el directorio ***node_modules*** contiene todas las dependencias necesarias para ejecutar el proyecto.
El directorio ***src*** va a contener todo el código que escribiremos, el cual contendrá módulos, componentes, directivas, etc.

El archivo ***Angular.json*** contiene la configuración que requiere ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) .
El archivo ***package.json*** contiene la configuración de nuestra aplicación, es decir: nombre, dependencias, scripts, etc.

El archivo ***tsconfig.json*** contiene la configuración de ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white).

El directorio ***src*** > ***app*** es donde crearemos los componentes, módulos, etc.

El directorio ***assets*** es utilizado para almacenar todos los recursos que utilizara la aplicación, tales como: **scripts e imágenes**, entre otros.

El directorio ***enviroments*** es utilizado para almacenar configuraciones globales, tales como variables de entorno para desarrollo y producción.

Abriremos la terminal de ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) para ejecutar el proyecto de ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white). 

En ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) automáticamente nos posiciona el directorio donde se encuentra el proyecto.

Para ejecutar el proyecto hacemos uso del comando:

```bash
ng serve
```

[![ejecucion-Proyecto.png](https://i.postimg.cc/7LJC7gXq/ejecucion-Proyecto.png)](https://postimg.cc/8FDPgfqY)
Damos clic en el link http:///localhost:4200/ y nos llevara a la siguiente pagina:

[![pagina-Mi-Primera-App.png](https://i.postimg.cc/cC06VPWJ/pagina-Mi-Primera-App.png)](https://postimg.cc/7Gtxzsfv)
Que realmente esta es una vista que  ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) nos muestra inicialmente.

El archivo *app.component.html* contiene el diseño y vista de la pagina que ya vimos anteriormente, vamos a borrarlo, guardamos y veamos lo que nos muestra el navegador:

[![pagina-Mi-Primera-App-Vacia.png](https://i.postimg.cc/BnYYtG7d/pagina-Mi-Primera-App-Vacia.png)](https://postimg.cc/18FcYbQH)
Ahora esta en blanco y también notamos que automáticamente se ven reflejados los cambios.

Vamos a crear un nuevo  componente, para ello necesitamos abrir una nueva terminal, presionamos sobre el botón con el símbolo + (mas).

En la terminal escribimos el comando:

```bash
ng generate component nombre_del_componente
```

En este caso se llamara:

```bash 
ng generate component nuevoComponente
```

Se deben agregar los componentes a un modulo para que ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) los reconozca.

Ademas en el nuevo directorio nuevoComponente tiene los tres archivos que se habían comentado, un ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white), un ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) un ***.ts*** y hay un cuarto archivo que se utiliza para hacer pruebas unitarias, es decir, pruebas por cada componente.

Para agregar un componente vamos a abrir el archivo ***.ts*** del componente creado .
En la clase del componente se puede ver que por encima tiene un decorador *@Component*  estos son usados para agregar funcionalidad a una clase:

```TypeScript
import { Component } from '@angular/core';
@component({
selector:'app-nuevo-componente',
standalone: true,
imports: [],
templateUrl: './nuevo-componente-component.html',
styleUrl: './nuevo-componente.component.scss'
})
export class NuevoComponenteComponent {

}
```

Por eso la propiedad ***templateUrl*** apunta al archivo *html*, con la cual enlaza el ***.ts*** con el *html*!.
[![abrir-Ts-Del-Componente-Creado.png](https://i.postimg.cc/85Vrmssx/abrir-Ts-Del-Componente-Creado.png)](https://postimg.cc/Y4b9pr6x)
El texto que pongamos en el componente se vera reflejado en la pagina, y que pasaria si mandamos llamar varias veces el componente?: 

```html
<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>

<app-nuevo-componente></app-nuevo-componente>
```

[![mandar-Llamar-Componente-png.png](https://i.postimg.cc/yxpChQ7x/mandar-Llamar-Componente-png.png)](https://postimg.cc/dZCfw9kc)
El componente renderiza el numero de veces que se manda a llamar.

Se le conoce como ***Binding*** a la unión de las propiedades entre el archivo ***.ts*** y el ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) de los componentes.

Ahora en: nuevo-componente.component.ts usamos el siguiente código creando un atributo en la clase llamada *name*, posteriormente se le asigna un valor en el método *ngOnInit*, este método se manda a llamar cuando se crea el componente..
Para saber el valor del atributo *name* en ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white), hacemos uso de las dobles llaves y dentro escribimos el nombre del atributo:

```TypeScript
import { Component, OnInit } from '@angular/core';


@Component({

selector: 'app-nuevo-componente',

standalone: true,

templateUrl: './nuevo-componente.component.html',

styleUrls: ['./nuevo-componente.component.scss']

})

export class NuevoComponenteComponent implements OnInit {

name: string = '';


constructor() { }


ngOnInit(): void {

this.name = 'Braulio Rodriguez'

}
}
```

```html
<h1>Mi primer componente</h1>

<p>
Valor del atributo name:{{ name }}
</p>
```

[![ngOnInit.png](https://i.postimg.cc/76N0Pck5/ngOnInit.png)](https://postimg.cc/DJ88Bxmh)
Luego para que el componente se vea reflejado en la pagina localhost: hay que poner la etiqueta solo en este caso ya que así se llama el componente:

```html
<app-nuevo-componente></app-nuevo-componente>
```

Para que de cierta manera se imprima en la pagina.

En pocas palabra se debe hacer todo esto:

[![componente-Para-Mostrar-En-Local-Host.png](https://i.postimg.cc/GtQWQc1b/componente-Para-Mostrar-En-Local-Host.png)](https://postimg.cc/RJWpCxFY)
