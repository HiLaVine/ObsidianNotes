Alcance de las [[Variables]], [[Funciones]] o bloque de código es un código, y de donde a donde son visibles.
También hay que tener en cuenta la [[Indentación]]. 
## Bloque de programa (program blocks)

### **let** y **const**

Para el uso de **let** y **const** en los bloques de programa tenemos algunos puntos o reglas a tomar en cuenta que son las siguientes:

1. Primera regla: Si declaramos una variable o constante cualquiera, usando let y const, fuera del bloque, estas seran conocidas como variables globales. Ya que se podran usar tanto dentro como fuera del bloque y en cualquier funcion. Las podemos referir por su nombre y por supuesto acceder a sus valores. Como en el siguiente código. 
~~~js
let height = 180;
{
    let weight = 70;
    console.log(height); // -> 180
    console.log(weight); // -> 70
}
console.log(height); // -> 180
console.log(weight); // -> Uncaught ReferenceError: weight is not defined
~~~

Donde vemos que la variable "height" es una variable global, al estar fuera del bloque. Y que "weight" es una variable local. El scope esta limitado por el bloque donde esta declarada. 
Y eso ve se mas claramente en el siguiente ejemplo:

~~~js
let  height  =  200;
{
         let  weight  =  100;
         {
                 let  info  =  "tall";
                 console.log(height);  //  ->  200
                 console.log(weight);  //  ->  100
                 console.log(info);  //  ->  tall
         }
         console.log(height);  //  ->  200
         console.log(weight);  //  ->  100
         console.log(info);  //  ->  Uncaught  ReferenceError:  info  is  not  defined
   }
~~~

Donde tenemos la variable info, que solo es visible dentro del bloque mas interno, y que las otras variables son visibles dentro de sus niveles. 

### **var**

En el caso de la palabra reservada var que ya pertenece a una versión de JavaScript vieja, al declarar una variable con este método, lo que tenemos es que todas las variables son globales, y no se respeta el scope antes mencionado. 

~~~js
var  height  =  180;
{
         var  weight  =  70;
         console.log(height);  //  ->  180
         console.log(weight);  //  ->  70	
}
console.log(height);  //  ->  180
console.log(weight);  //  ->  70
~~~

Esto no es implícitamente malo, ya que el único momento donde si podremos declara una variable con **var** es en las [[Funciones]]. Ya que **var** al estar dentro del bloque de una función, dicha variable solo se podrá usar dentro de la misma función, como si fuera con **let**. 

