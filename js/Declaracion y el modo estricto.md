En JavaScript existen cosas curiosas que normalmente llevan a errores. Y uno de ellos es el caso siguiente al momento de [[Declarar Variables]]

~~~JS
height = 174;
console.log(height); 
~~~

En el caso anterior vemos que no tenemos **let** para la declaración de la variable y esto no causa ningún problema al momento de ser interpretado. Pero esto puede causar problemas  de ambigüedad y generar situaciones erróneas. 

Por lo que podemos agregar lo siguiente: 

~~~JS
"use strict";

height = 174;
console.log(height); //height is not defined
~~~

Con esta modificación podremos observar que ahora si nos marca el error de que height no esta declarada. 

Al colocar **"use strict";** lo que hacemos es forzar al interprete a comportarse de acuerdo a los estándares modernos de JavaScript y evita que se cometan estos errores en JS. 

Esta sentencia debe colocarse siempre al inicio ya que JavaScript es un lenguaje interpretado. 