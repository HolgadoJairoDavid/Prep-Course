* Funciones Callback

Funciones callback, es la denominación que reciben las funciones que son pasadas como argumentos de otras funciones. El nombre se debe a una convención que se estableció entre programodores, como así también, el hecho de que, en el argumento se escriba como 'cb'. 

Son conocidas, además, como "devoluciones de llamadas", las cuales nos brinda un abanico de herramientas a la hora de programar. 

Ejemplo:

> function esteEsUnCallback(marcaDeAuto){
    return 'Este es un auto de marca ' + marcaDeAuto;
}

> function recibeCallBack(marca, cb){
    return cb(marca);
}

> recibeCallback('Lamborghini', esteEsUnCallback)
> 'Este es un auto de marca Lamborghini'