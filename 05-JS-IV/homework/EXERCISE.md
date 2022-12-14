* Objetos:

Los objetos son una colección de propiedades. Surgieron para cubrir el principal objetivo de JavaScript de resolver dificultades de la vida real. Para comprender mejor sus pricipios podemos citar un elemento y, a partir de él, analizar sus características.

Por ejemplo, un auto con 0 Km de recorrido. Cuya marca es "Rodini", con ruedas de 2.5 bares de presión, de color gris oscuro, con un terminado de pintura mate. La velocidad máxima a la que llega es de 355 Km/h y acelera de 0 km/h a 100 km/h en tan sólo 5.91 segundos. 

Como podemos observar, es información relativamente compleja para almacenar dentro de una variable o un array, debido a la naturaleza propia de dichas herramientas de JavaScript. Sin embargo, no lo es así con los objetos. Siguiendo el ejemplo anterior podemos realizar la siguiente sintaxis:

> var objetoAuto = {
    dueño: true,
    marca: 'Rodini',
    recorridoActual: '0 Km',
    presiónEnRuedas: '2.5 bares',
    color: 'gris oscuro',
    pinturaTerminado: 'mate',
    velocidadMáx: '355 km/h',
    aceleraciónDeCeroACien: '5.91 seg'
}

Para iniciar un objeto, debemos declarar una variable. Y, a la hora de asignar el valor, este debe ir entre llaves. Esto es lo que le permitirá saber a nuestro computador con qué vamos a trabajar en las siguientes líneas de código. Seguido de ello, se declaran las propiedades. En primer lugar, se coloca el nombre de la propiedad acompañado de ":" (dos puntos), lo que nos permitirá asignar el valor correspondiente (que puede ser de cualquier tipo, incluso otros objetos, arrays y/ o funciones). Por último, cada uno de las propiedades deben de estar separadas por medio de una coma. 

* Propiedades:

Son las asociaciones entre un nombre (o clave) y un valor. Es decir, es la relación "Key- Value".

Por ejemplo:

// dueño: true

Dichas claves, pueden ser strings que, a su vez, permiten acceder a los valores de las propiedades pertinentes. Para ello debemos utilizar la notación DRY CODE (notación de puntos) o BRACKET NOTATION (notación de corchetes). 

* Notación de puntos vs notación de corchetes:

Para la notación de puntos, sólo debemos indicar el nombre del objeto y la clave de la propiedad correspodiente.

Ejemplo:

> objetoAuto.marca
> 'Rodini'

Mientras que, para la notación de corchetes, debemos establecer el nombre del objeto, con la diferencia de que la clave debe ir entre comillas simples.

Ejemplo: 

> objetoAuto['dueño']
> true


* Métodos:

Los métodos son propiedades cuyo valores son funciones. A nuestro objeto creado en las líneas anteriores, podemos agregarle el siguiente método.

> objetoAuto['esteEsUnMétodo']= () => {console.log('Este auto fue vendido a las 07:55 AM')};
> objetoAuto.esteEsUnMétodo()
> 'Este auto fue vendido a las 07:55 AM'

* Bucle `for…in`:

Es una herramienta de tipo bucle que nos permite iterar sobre cada par clave- valor de un objeto. 

Ejemplo:

> for(let clave in objetoAuto){
    console.log(clave + ": " objeto[clave]);
}

> 'dueño: true'
> 'marca: Rodini'
> 'recorridoActual: 0 Km'
> 'presiónEnRuedas: 2.5 bares'
> 'color: gris oscuro'
> 'pinturaTerminado: mate'
> 'velocidadMáx: 355 km/h'
> 'aceleraciónDeCeroACien: 5.91 seg'

