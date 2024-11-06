
En Kotiln, se tienen 2 palabras clave para definir variable: val y var. 

Para declarar una variable con val: 

~~~kotlin
//val nombreVariable : tipodeDato = valor;
val contador : int = 5;
~~~

En la sentencia anterior definimos una variable llamada contador de tipo entero y en valor de 5.

Lo tipos de dato mas comunes en kotlin son:

| String    | Cadena                                       |
| --------- | -------------------------------------------- |
| int       | Valores enteros                              |
| Double    | numeros con punto decima                     |
| Float     | Números con punto decimal de mayor precisión |
| Bolean    | Con valor de True o False                    |
| Character | Un caracter                                  |

Podemos declarar una variable con val sin inicializarla desde el inicio pero hay que definir el tipo de dato. 

~~~kotlin
val cad : String;
.
.
.
cad = "hola";
~~~

## Inferencia de tipo

Es cuando el compilador de Kotlin puede inferir (determinar) que tipo de dato debe ser una variable, sin que el tipo se escriba de forma explicita en el código. 

~~~kotlin
val x = ;
val cad = "hola";
println(x);
printn(cad);
~~~

Si se necesita actualizar el valor de variables, se utiliza en la declaración var en vez de val. Con var la variable es mutable y se utiliza igual que val. 

~~~kotlin
var y = 9;
var cad = "adios";
var num : int = 15;

var y = 10;
var cad = "hola";
var num : int = 11;
~~~






