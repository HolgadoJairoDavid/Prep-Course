* bucles 'for':

En JavaScript, es un statement que permite realizar tareas repetitivas, es decir, repetir bloques de código muchas veces. Es debido a esta peculiridad que es muy importante a la hora de programar con este lenguaje. 

Una de sus frases características es "Don't repeat yourself". 

Ejemplo: 

> function NumbersFromOne (N) {
    for (var i = 0; i < N; i++){
        return i;
    }
}

Para este ejemplo, podemos apreciar que se ha hecho uso de una función para establecer un bucle for. Este último está constituido por la palabra clave 'for', seguida de una declaración que va entre paréntesis. 

Entre paréntesis, debemos aclarar una variable específica (i= iteración), una corte del bucle (i < N, en este caso)e indicar que las iteraciones vayan en aumento (i++). Para finalizar, se coloca "return", tanto para detener la función y retornar el valor correspodiente de cada iteración. 

> NumbersFromOne(10)
    0
    1
    2
    3
    4
    5
    6
    7
    8
    9

Dentro de un bucle for, podemos anidar otros bucles for, en caso que lo que necesitemos. 

> function buclesAnidados (n) {
    // supongamos que 'n' es un array de arrays. 
    for (let i = 0; i < n.length; i++){
        for(let j = 0; j < n[i].length; j++) {
            if (n[i][j] === 7) return true;
        } 
     }
}

* &&, ||, !

Estos son conocidos como operadores lógicos. Cada uno de ellos tiene un significado distinto y cumplen operaciones diferentes, que se convierten en valores booleanos ('true' o 'false'). 

Por lo general, siempre involucran la participación de dos valores o variables.

Comencemos por '&&' (AND). La operación que realiza es corroborar que ambos valores involucrados sean verdaderos, para que el resultado final sea true. De lo contrario será false.

Ejemplo:
	2 === 3 && 3 === 3 // retornará false, ya que 2 no es igual a 3.

Por otra parte, ‘||’ (OR) es el operador que se encarga de analizar de que, si al menos uno de los valores involucrados es verdadero, el resultado final es true. Mientras que, si los dos son falsos, resultará en false.
Ejemplo:
	2 === 3 || 3 === 3 // retornará true, ya que al menos 3 sí es igual a 3.

Por último, ‘!’ (NOT) es el encargado de convertir un valor verdadero en falso y viceversa. Esto afectará de manera proporcional, en el resultado final de la operación. 

Ejemplo:
	2 !== 3 // retornará true. Debido a que, al establecer que 2 no es igual a 3, se convierte en una expresión verdadera. 

Para comprender mejor sus diferencias, podemos observar la siguiente "TABLA DE LA VERDAD":


 a         b      a && b    a || b       !a
true      true     true      true       false 
true      false    false     true       false
false     true     false     true       true
false     false    false     false      true