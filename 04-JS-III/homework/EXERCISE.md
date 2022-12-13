* Arrays:

Es un tipo de contendor, conocido también como matriz o areglo, que puede recibir cualquier tipo de datos (funciones y arreglos, inclusive), cuya colección es infinita, es decir, que podemos colocar la cantidad que deseemos. 

Ejemplo: 

var arrayEjemplo = [1, 2, 3, 'Jairo', true, 1 !== 9, let unica = () => console.log('hola'), [5, 6, 7, 3], 'mundial'];

Como podemos ver, para establecer un array sólo debemos declarar una variable y, la asignación que realicemos debe estar entre corchetes. Los elementos que van dentro de la matriz se separan por medio de una "," (coma).

Los elementos de un array, están ordenados por un índice que comienza a contar desde el "0" (cero). Es por esto que, para acceder a los elementos de un array, podemos hacerlo de la siguiente manera. 

> arrayEjemplo[0]
// nos retornará:
> 1
// ya que es el primer elemento de este array.Y así sucesivamente con los demás datos. 

Los arrays tienen muchos métdos integrados. Uno de los más utilizados es ".length", el cual nos permite conocer la cantidad de elementos dentro de un array. 

Ejemplo:

> arrayEjemplo.length 
> 9