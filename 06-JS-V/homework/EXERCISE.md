* `prototype`:

Es un mecanidsmo que nos permite crear métodos dentro de una clase de objetos o que estos últimos los hereden. Como sabemos, a las clases podemos observarlas como clasificaciones de objetos, a partir de de las cuales se pueden crear objetos que compartan ciertas PROPIEDADES. 

Por ejemplo: 

Necesitamos crear 7 objetos, que comparten el hecho de que son libros. 

Para ello podemos establecer la siguiente clase.

> function Libros (nombre, clasificación, autor, edición, impresión) {
    this.nombre= nombre;
    this.clasificación= clasificación;
    this.autor= autor;
    this.edición= edición;
    this.impresión= impresión
}

Como podemos observar, no podemos colocar una función dentro de otra para crear un método. Sin embargo, podemos realizar lo siguiente: 

Libros.prototype.getNombre = function () {
    return 'Este libro se llama ' + this.nombre +'.';
}

De este modo, todo los objetos que se creen con la clase Libros, tendrán contenido en su 'prototype' el método 'getNombre'. Además, se logra apreciar que presenta una sintaxis sencilla y fácil de comprender.

> var classifiedBookOne= new Libros('Escribir en tiempos de pandemia', 'Cuentos', 'Estudiantes de secundaria', 2020, 2021)

* _Constructors_ (de Clases):

Es un método especial que ofrece la posibilidad de crear e inicializar un objeto construido a partir de una clase. Según la última actualización de JavaScript, "ECMAScript 6" (ES6), se presentó una nueva forma de declarar una clase. 

Por ejemplo:
// Antes de continuar, es importante aclarar que, a la hora de establecer una clase, existe una convención entre programadores de que, al inicio siempre se escriba con mayúscula. De este modo, el código que se trabaje en grupos, es más llevadero. 

> class LibrosSinClasificar {
    constructor (nombre, autor, edición, impresión){
        this.nombre= nombre;
        this.autor= autor;
        this.edición= edición;
        this.impresión= impresión 
    }
}

> var oneBook= new LibrosSinClasificar('Días lluviosos', 'Gabriel García Márquez', 1985, 1987);