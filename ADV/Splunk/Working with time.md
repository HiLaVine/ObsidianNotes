
Cuando un evento es ingestado, se crea una marca de tiempo y se guarda en el campo _time. Y esto se usa para crear la inteface de tiempo (timeline) que usa splunk en su interfaz de usuario.

Este se guarda con los otros campos default, host, source y sourcetype. Y están expresadas en epoch time, que se traduce cada vez que se hace una búsqueda.

Todos los eventos se ordenan por tiempo.

El campo _time, y otros campos de metadata (host, source, sourcetype e index) se asignan a cada evento, Siempre!!

Se ajusta a tu zona horaria.

La timeline (en la interfaz de usuario) se puede formatear para darle un eje x e y completo.

Con el Zoom to selection, podemos hacer zoom xd para ver la información en ese horario de interés

earliest and latest time modifiers.

~~~splunk
… earliest=[+|-]<timeInt><timeUnit>@<timeUnit>  
… latest=[+|-]<timeInt><timeUnit>@<timeUnit>
~~~

Default time fields

## Formating time

Se puede definir como el tiempo se formatea en los resultados de las búsquedas usando las funciones de tiempo.

#### Comando eval

Este es un comando muy útil que te permite escribir los resultados de una expresión en un nuevo campo o uno preexistente.

con este comando se pueden usar el now() que regresa el tiempo en el que se inicio una búsqueda. Y time() que regresa el tiempo que tardo en procesarse un evento por el comando eval.