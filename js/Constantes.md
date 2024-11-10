Las constantes son [[Variables]] que no se pueden modificar una vez inicializadas. Y se declaran con la palabra reservada **const**. Y estas al contrario de las otras variables no se pueden inicializar después de declararla. 

~~~js
const greeting = "Hello!!";

const greeting; // -> Uncaught SyntaxError: Missing initializer in const declaration
greeting = "Hello!!"
~~~

Como se menciono antes, las constantes no se puede modificar su contenido y tenemos de ejemplo lo siguiente: 

~~~js
const greeting = "hello";

greeting = "hi"; // -> TypeError: Assignment to constant variable.
~~~

El objetivo principal de las constantes es erradicar la posibilidad de accidentalmente modificar un valor ya guardado. Y también se puede usar para hacer cálculos que siempre va a necesitar ese valor o enviar un mensaje que lo necesite. 