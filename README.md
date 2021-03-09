# clone-instagram-with-sass
_A small project to get use to SASS. The goal will be to hard-code the login and main page of instagram and apply it's styles using SASS._

# Theoretical part

_The following questions will be answered with my own words to check the understanding of the main SASS concepts:_

- ### What is SASS? What does SASS stand for?
Se trata de un pseudo-lenguaje de prgramación para escribir código CSS. 
Syntactically Awesome Stylesheets
- ### What is a CSS pre-processor?
Se trata de un proceso intermedio de traducción de un lenguaje
- ### What does a pre-processor have to do with SASS?
El navegadorr no entiende SASS, entiende CSS. De este modo hay que pre-procesar(traducir) SASS a CSS para que este pueda ser leido e interpretado por el navegador
- ### Why use SASS?
Al introducir variables, condicionales, bucles, herencia, etc, facilita enormemente la escritura de estilos para el desarrollo web.
Además, comparado con otros pre-procesadoes, es el que cuenta con mayor nº de usuarios ypor ende con una mayor comunidad y documentación
- ### SASS has disadvantages? Which are?
Hay que aprender a usar la herramienta y su sintaxis es algo más compleja que el puro CSS.
Además al añadir esta etapa intermedia de compilación de SASS a CSS existe un pequeño tiempo de demora extra si el archivo es muy grande
- ### What is a SASS Variable? Explain why are useful
Al igual que en cualquier otro lenguaje de programnación, una variable es un nombre simbólico en el que se puede almacenar un valor y reutilizarlo a lo largo del código
- ### Explain the SASS variables property with an example
Los únicos valores que se pueden almacenar en una variables de SASS son propiedades CSS.

```
$font-stack: Helvetica, sans-serif;
$primary-color: #333;

body {
font: 100% $font-stack;
color: $primary-color;
}
```
- ### What is a mixin? Why is it important? Give an example
Es una porción de código reutilizable. Es importante porque nos permite no duplicar código, generando hojas de estilo menos pesadas. Un mixin es análogo a una función en lenguajes de programación
- ### What is SCSS? Give an example
Es una nueva versión de SASS.
Tiene su propia extensión .scss y es 100% compatible con CSS (puedes escribir ambos en el mismo fichero)
- ### What is the difference between .scss and .sass syntax.
SCSS utiliza brackets al igual que CSS tradicional, mientras que SASS hace uso de identación. Además en SASS no es necesario poner ; al final de cada regla
- ### In which cases would we use SCSS? And in which cases would we use SASS?
Usaría scss para poder escribir código junto a css, ya que son totalmente compatibles. En caso contrario usaría sass
- ### Explain how traditional CSS and Preprocessed CSS workflows are different
CSS es estrictamente secuencial, donde el orden de dónde está escrita cada línea es vital para el funcionamiento de la cascada de la hoja de estilos. En SASS sin embargo, aunque el orden también es importante, puedes tener tener una regla cuyo valor se lo indicas a través de una variable que ha sido definida más arriba, o un bucle que ejecuta de nuevo las mismas líneas, etc.
- ### Can we create functions with SASS? If it is true, give an example
En SASS no existen las funciones como tal, pero existen algo muy parecido llamado mixin
```
@mixin transform($property) {
-webkit-transform: $property;
-ms-transform: $property;
transform: $property;
}
.box { @include transform(rotate(30deg)); }
```
- ### What is nesting? Is it useful? Give an example of nesting
El nesting es una forma de escribir código sass que permite establecer una herencia y una jerarquía respecto a los elementos a los que se les está aplicando los estilos
``` 
nav {
ul {
margin: 0;
padding: 0;
list-style: none;
}
li { display: inline-block; }
a {
display: block;
padding: 6px 12px;
text-decoration: none;
}
}
```
- ### Why use @import?
Los imports eran una manera de incluir partes de código de otros ficheros u otros ficheros enteros en el fichero desde el que se realiza el import. Sin embargo esta forma de trabajar está anticuada y en la actualidad se recomienda uar @use y @extend
- ### How can we import other CSS/SASS files in SASS? Give an example
Se utiliza escribiendo @import seguido del nombre del archivo que se quiere importar (sin extensión y entrecomillado).
Sin embargo no se recomienda hacer uso de imports
- ### Explain the concept of inheritance in SASS
La herencia nos permite reutilizar código de forma que no haya código duplicad y el archivo no quede tan extenso
- ### Why use @extend? Give an example
Gracias @extend podemos hacer uso de la herencia para aprovechar sus ventajas:
```
%message-shared {
border: 1px solid #ccc;
padding: 10px;
color: grey;
}
.message {
@extend %message-shared;
}
.success {
@extend %message-shared;
border-color: green;
}
```
