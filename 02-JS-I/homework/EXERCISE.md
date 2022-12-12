* Variables:

Es una manera de guardar o almacenar un valor, que podrá ser utilizado más tarde. Por ende, podemos compararla con una caja en la que deseamos colocar determinados valores. Hay dos tipos de variables. Las que nos ofrecen la posibilidad de sobrescribir valores y restablecerlos a cualquier tipo y las que no.

Dentro del primer grupo, se encuentran "let" y "var". Para declarar la variable "var", sólo debemos establecer la palabra clave "var", seguida del nombre que deseamos otorgarle, un signo "=" (igual a) que, en estos cosas adquiere un sentido de asignación y no de igualación. Del mismo modo sucede con "let". Sólo que se diferencia de la variable "var", en que el alcance de esta última es global. Mientras que, de "let" es en un scope específico. 

Dentro de la segunda clasificación, está "const". Esta variable se declara de la misma manera que las anteriores, con la diferencia de que, su denominación es única y su valor no se uede sobrescribir.

Ejemplo: 
        >  var Jairo = 18;
        > let apellido = 'Holgado';
        > const segundoNombre = 'David';

* Strings:

Es un tipo de valor en JavaScript, que se compone por cadena de textos. Siempre debe ir entre comillas simples o dobles. 

Ejemplo:

            'Jairo' (String).

            Jairo  (No es String).

* Funciones:

Son un conjunto de códigos muy importantes en JavaScript, que permiten realizar determinadas tareas o calcular valores. 

Ejemplo: 

           > function sumar (a, b) {
                return a + b;
            }

Este mismo ejemplo nos permitirá analizar la anatomía de una función. Para declararla, debemos iniciar con la palabra clave function. Luego debemos otorgarle un nombre, en este caso es "sumar". Y, según lo que requiera la tarea que necesitemos ejecutar, colocaremos el argumento correspondiente entre los paréntesis pertinentes, tal como lo hicimos con "(a, b)". Por último, podemos observar a "return". Es una declaración que da fin a la función y permite retornar lo que haya dentro de la función. 

> sumar (1,2);

Nos retornaría= 
                3.

Otras formas de declarar una función son las siguientes:

> var sumar1 = (a, b) => a + b; 

[Esta es conocida como función flecha, que se caracteriza tanto porque no hay necesidad de usar la declaración "return", como así también porque inicia con una variable].

> var sumar2 = function (a, b) {
    return a + b;
}

[En este caso utilizamos una variable para declarar una función].

* Declaraciones 'if':

Son aquellas que se especializan en el control de flujos, para verificar si algo es true o false, de manera especial dentro de una función. 

Ejemplo: 

> function primerNombre(nombre) {
    if (nombre = 'Jairo') {
        return true;
    }
    return false;
}

> primerNombre ('David')
> false

 * Valores booleanos (`true`, `false`)

 Son un tipo de valor que se utilizan para declarar si algo es verdadero ('true') o falso ('false'). 

 Ejemplo: 

> 1 + 1 === 3;
> false

> var Edad = 19;
> Edad > 18;
> true

> 5 * 5 === 25;
> true