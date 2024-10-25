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

