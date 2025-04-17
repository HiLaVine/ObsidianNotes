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
  drwxrwxrwx para un directorio
  -rwxrwxrwx 
~~~

- En la cadena anterior el primer caracter "d" indica que se trata de un directorio. Pero si tuviera un - seria un archivo normal.
- Los siguientes 3 caracteres "rwx" representan los permisos del usuario, r significa que puede leer, w qu epuede escribir y x que puede ejecutar. Cuando no tiene alguno, tendra un guion.
- Los siguientes 3 indican los permisos del grupo, en este caso son los mismos del usuario.
- Y los ultimos 3 son los permisos de los otros usuarios, y que tambien tienen todos los permisos. 

## Cambiar permisos de ususario

Para esto se usa el comando chmod, y existen dos modos para cambiar los permisos. 

~~~Bash
  chmod g+w,o-r access.txt
~~~
Desglozando el comando tenemos los siguientes puntos:

- access.txt -> el archivo a el cual se le haran los cambios de permisos.
- g+w, o-r -> indica como se van a cambiar los permisos. 
  - En este comando hay que recordar que user = u, group = g y others  = o.
  - y que + y - indican si se añaden o quitan permisos.
  - Por lo tanto tenemos que:
      - g+w -> nos indica que a el group (g) se la añaden permisos de escritura (w)
      - y que a others (o) se le quitan permisos de lectura (r).

## Agrega y elimina usuarios

Root user: Un usuario con privilegios elevados para modificar el sistema. 

Sudo -> Super user do

useradd -> comando para añadir usuarios al sistema.

un ejemplo para añadir un usuario seria

~~~Bash
  sudo useradd salesrep7
~~~

O para eliminarlo seria: 

userdel -> eliminar un usuario

~~~Bash
  sudo userdel salesrep7
~~~

## Paginas dentro de shell

man: muestra informacion en la pantalla sobre otros comandos y como funcionan

whatis: muestra informacion del comando en una sola linea

apropos: busca la descripcion de un string en especifico dentro del manual, como seria 

apropos password y va a mostrar en el manula todas las lineas para password. y con -a se puede añadir otro string


