Como se menciono antes las [[Variables]] solo reservan un nombre. Aunque técnicamente es mucho mas complejo ya que tiene que ver directamente con el uso de memoria. En JS no vamos a pensar casi nunca en esta parte.  

El valor guardado en las [[Variables]] puede ser modificado, a lo largo del programa.  Ya que podemos declarar variables que no se pueden modificar, y tienen el nombre de [[Constantes]]

Para la declaración usamos **var** o **let** para las variables y para las constantes usamos **const**. 

Y la única diferencia que encontramos entre **var** y **let** es que con la primera podemos definir la misma variable (mismo nombre) las veces que sea necesaria. Y con la otra no se puede hacer esto y se marcara error si lo hacemos. 

~~~JavaScript
//Tienen el mismo nombre y no se marca error. 
var height; 
var height;
//Tienen el mismo nombre y se marca error.
let weight; //Identifier 'height' has already been declared
let weight;
~~~

