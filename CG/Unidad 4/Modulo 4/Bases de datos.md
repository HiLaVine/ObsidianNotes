## ¿Qué es una base de datos?

Es una colección organizada de información o datos. Estas estan dieseñadas para que una gran cantidad de usuarios puedan acceder a la vez a ella y almacenar grandes cantidades de datos. 

Existen muchas formas de bases de datos, y una de las mas usadas es la base relaicional. 

### ¿Qué es una base relacional?

Esta es una base de datos que se estructura con tablas relacionadas entre si. Estas tablas tienen campos de información, como el ejemplo siguiente: 

|empleados|
|-----------|
id_empleado
id_dispositivo
nombre_usuario
departamento
oficina

Además, las tablas contiene filas, tambien llamdas registros. Estas tienen datos específicos relacionados con las columnas. Como en el siguiente ejemplo

|id_empleado|id_dispositivo| nombre_usuario| departamento| oficina|
|-----------|--------------|----------------|------------|---------|
| 1000 | a320b137c219 | elarson | Marketing | East-170|


Las bases de datos relacionales suelen tener varias tablas. 

Las columnas que relacionan dos tablas entre si se llaman claves. Y existen dos tipo de claves: 
- Primary key: Una columna donde todas las filas tienen una entrada unica.
- Foreing key: Una columna de una tabla que en otra tabla es una primary key.

**Nota:** Cada tabla solo puede tener una clave primaria, pero varias foraneas. 

## SQL

SQL o Structured Query Language es un lenguaje de programación usado para crear, interactuar y pedir información de una base de datos. 

Pero primero que es una Query (consulta): es una peticion de datos a una tabla de una base de datos o a una combinacion de tablas. 

Para recuperar un registro o log que recordando es un conjunto de eventos que han pasado en una organización.

### Consultas 

Para llevar a cabo cualquier consulta de informacion con SQL de una base de datos se usan los dos comandos más básicos, SELECT y FROM. 

El primero (SELECT), indica que informacion es la que se esta consultando. 

Y el segundo (FROM), indica de que tabla se va a hacer esa consulta. 

Para llevar a cabo las consultas se debe respuestar la sintaxis de SQL, que son las reglas que determinan que es correctamente estructurado en un lenguaje de computadoras. 

Un ejemplo de una consulta seria:

~~~SQL
  SELECT employee_id, device_id
  FROM employees;
~~~

Que nos devuelve el id del empleado y del dispositivo de la tabla empleados. 

### Filtros Básicos

El filtrado consiste en seleccionar datos que coincidan con una condición. 

Para indicar que se va a usar un filtro, usamos la palabra clave WHERE, que indica la condición del filtro. 

En este caso, lo que hacemos es poner la palabra WHERE seguida del filtro que se va a usar. 

Como por ejemplo la siguiente consulta, donde buscamos solo los que pertenezcan a USA. 

~~~SQL
  SELECT *
  FROM log_in_attemps
  WHERE country  = 'USA';
~~~

Otro filtro es usar el signo "%" para buscar un **patrón**, como por ejemplo East% donde se va a encontrar todo lo que empiece por East. 

Y para esto usamos la palabra LIKE, en vez del signo =.

Quedando un ejemplo de la siguiente forma: 

~~~SQL
  SELECT *
  FROM log_in_attemps
  WHERE country  LIKE 'US%';
~~~

### Comodines

Los comodines son un caracter especial que se puede sustituir por cualquier otro caracter. Dos de los comodines mas utiles son el signo de porcentaje % y el guion bajo _
- El primero (%), puede sustituir cualquiera de los demas caracteres.
- El segundo (_), solo puede sustituir uno de las demas caracteres.

Puedes colocar estos comodines depues de una cadena, antes de una cadena o en ambas ubicaciones, dependiendo el patron buscado. 

| Patrón | Resultados que va a devolver |
|--------|------------------------------|
| 'a%' | apple123, art, a |
| 'a_' | as, an , a7 |
| 'a__' | ant, add, alc |
| '%a' | pizza, Z6ra, a |
| '_a' | ma, la, Ha |
| '%a%' | Again, back, a |
| '_a_' | car, ban, ea7 |



