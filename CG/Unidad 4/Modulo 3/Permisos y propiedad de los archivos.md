Un permiso es el tipo de acceso que se da a un archivo o directorio. Estos se relacionan con el concepto de dar acceso a recursos especificos. 

Hay tres tipos de permisos en linux, que un usuario autorizado puede tener. 

- Permiso de lectura: en este solo se permite leer el contenido de los archivos.

- Permisos de escritura: en este no solo se puede leer el contenido, si no tambien hacer modificicacionesdentro.

- Permisos de ejecución: permiten ejecutarlo si este es ejecutable.

Y Tambien existen tres tipos de propietarios:

- Usuario: el propietario del archivo.
- Grupo: cada usuario es parte de un grupo.
- Otros usuarios: se refiere a usuario fuera del sistema (osea fuera del grupo)

En linux los permisos de los usuarios estan representados por una cade de 10 caracteres. 

Ejemplo: 

~~~Bash
  drwxrwxrwx
~~~

- En la cadena anterior el primer caracter "d" indica que se trata de un directorio. Pero si tuviera un - seria un archivo normal.
- Los siguientes 3 caracteres "rwx" representan los permisos del usuario, r significa que puede leer, w qu epuede escribir y x que puede ejecutar. Cuando no tiene alguno, tendra un guion.
- Los siguientes 3 indican los permisos del grupo, en este caso son los mismos del usuario.
- Y los ultimos 3 son los permisos de los otros usuarios, y que tambien tienen todos los permisos. 
