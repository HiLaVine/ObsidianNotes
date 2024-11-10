Como su nombre sugiere [[Variables]] pueden guardar datos que van a variar. Estos cambios se logran asignando un nuevo valor a la variable, con lo cual se sobrescribe el valor anterior con el nuevo. 

~~~js
let  steps  =  100;
console.log(steps);  //  ->  100

steps  =  120;  //  ->  120
console.log(steps);

steps  =  steps  +  200;
console.log(steps);  //  ->  320
~~~

**Coerción de tipo** en JavaScript. Cuando el operador `+` se encuentra con un string y un número, convierte el número en un string para realizar la concatenación.

~~~js
let greeting = "hello";
let counter = 100;

console.log(greeting + counter);
~~~

