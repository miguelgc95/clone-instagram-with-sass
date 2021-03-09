# clone-instagram-with-sass
A small project to get use to SASS. The goal will be to hard-code the login and main page of instagram and apply it's styles

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

```$font-stack: Helvetica, sans-serif;
$primary-color: #333;

body {
font: 100% $font-stack;
color: $primary-color;
}´´´

- ### What is a mixin? Why is it important? Give an example

- ### What is SCSS? Give an example

- ### What is SASS? Give an example

- ### What is the difference between .scss and .sass syntax.

- ### In which cases would we use SCSS? And in which cases would we use SASS?

- ### Explain how traditional CSS and Preprocessed CSS workflows are different

- ### Can we create functions with SASS? If it is true, give an example

- ### What is nesting? Is it useful? Give an example of nesting

- ### Why use @import?

- ### How can we import other CSS/SASS files in SASS? Give an example

- ### Explain the concept of inheritance in SASS

- ### Why use @extend? Give an example

