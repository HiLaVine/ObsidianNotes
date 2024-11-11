Una función cumple el objetivo de tener en un solo lugar una parte del código que se encarga de hacer algo, y que va a ser usada mas de una vez. El objetivo de esta es como con todo hacer mas fácil programar y evitar problemas como tener que modificar una parte del código que se uso muchas veces. 

En JS las funciones de declaran de la siguiente manera: 

~~~js
function  testFunction()  {
         console.log("Hello");
         console.log("World");
}
~~~

Donde en vez de declarar muchas veces lo que hay dentro de la misma, lo que hacemos es llamar a "testFunction()" siempre que sea necesario. 

A estas funciones también se le pueden asignar parámetros, que son los datos con los que va a hacer algo en caso de ser necesario. 

~~~js
function suma (a , b){
    console.log(a + b);
}
suma(9, 10);
~~~

