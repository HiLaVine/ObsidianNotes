Las clases en kotlin se declaran utilizando la palabra reservada "class"

~~~kotlin
Class Persona { ... }
~~~

la declaración de la clase consta del nombre de la clase y puede contener los parámetros del que se denomina constructor principal. Entre llaves se encuentra el cuerpo de la clase

## Constructores

La clase kotlin contiene un constructor principal y uno o mas constructores secundarios. 

~~~kotlin
class Persona constructor (nombre: String){ ... }
~~~

Si el constructor principal no tiene anotaciones ni modificadores de acceso se puede omitir la palabra constructor

~~~kotlin
class Persona (nombre: String){ ... }
~~~

El constructor principal inicializa las propiedades de una instancia de la clase y no puede contener otro código ejecutable. Si se requiere un código adicional para el constructor se utiliza el bloque inicializador especificado por la palabra "init". Durante la inicialización estos bloques se ejecutan en el orden que aparecen. 

~~~kotlin
class Persona (nombre: String){
	val nomUsuario = "Usuario 1";
	init{
		println("Primer bloque inicializador $nombre")
	}
	val edad = 20
	init{
		println("Segundo bloque incializador:" {$nombre.length})
	}
}
~~~

para crear una instancia de la clase se invoca al constructor de la clase como a una función. 

~~~kotlin
fun main(){
	val p1 = Persona("Luis")
}
~~~

Al declarar las propiedades en el constructor también podemos inicializarlas con un valor por default. 

~~~kotlin
class Persona (nombre:String="ana"){
	.
	.
	.
}
~~~

De forma similar las propiedades pueden ser declaradas con var o con val. 

## Constructores secundarios

Los constructores secundarios se identifican con la palabra 

~~~kotlin
class Circulo (val radio:Double){
	constructor (nombre:String):this(5.0)
	constructor(diametro:Int):this(diametro/2.0){
		println("constructor que recibe el diametro");
    }
	init{
		println("area:${PI*radio*radio}")	
	}
}

fun main(){
	val c = Circulo(3.5);
	val c2 = Circulo(2);
    val c3 = Circulo("uno");
}
~~~