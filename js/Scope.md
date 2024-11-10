Alcance de las [[Variables]], [[Funciones]] o bloque de código es un codigo, y de donde a donde son visibles.
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

Donde vemos que 