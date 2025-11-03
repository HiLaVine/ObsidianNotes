Comando chart

Este comando es usado para tomar los resultados y regresarlos formateados en una tabla.

chart command Split fields

Usar el over <row-split> para especificar el eje X  crear una serie simple de datos, para crear multiseries se usa el by <colum-split>

Los resultados solo pueden usar el Split usando dos campos.

## Timechart Command

Crea adiciones estadísticas contra el tiempo y regresa series basadas en el tiempo conde el _time siempre esta en el eje X

La principal diferencia entre chart y timechart es que timechart solo soporta un Split adicional y esto es porque el eje x esta segmentado automáticamente basado en el tiempo y el con el timechart se puede controlar el comportamiento usando el span y el limit.

## Top command

Este comando encuentra los campos mas comunes del resultado de tus búsquedas. Otra característica importante del comando TOP, es la habilidad de encontrar los valores top de combinaciones o campos específicos añadiendo mas de un campo a nuestra lista.

## Rare Command

Este comando tiene las mismas funciones que el comando top pero enfocado en la búsqueda de los campos con menos valores.

## Stats Command

Para producir estadísticas de nuestros resultados, este usa varias funciones para calcular estadísticas de nuestros resultados de búsqueda. La salida será en una tabla.

## Stats functions

Tenemos 4 categorías en las funciones del comando stats

- agregate: cuenta valores de los eventos para crear un solo valor (count(), distinct_count(), sum(), etc)  
- Event order: regresa los valores de los campos basado en el orden de procesamiento.  
- Multivalue: regresa una lista de valores para un campo como una entrada multi valor  
- Time: regresa los valores basados en tiempo.

## Eval command

Este se usa para hacer calculos con los valores en tus datos. Esta es capaz de crear un nuevo campo o modificar uno existente.

Esta incluye operaciones matematicas, concatenaciones de strings, comparacion de expresiones, expresiones boleanas, o llamada a funciones.

## Rename command

Cuando se incluyen espacios o caracteres especiales en los nombres de campos, se usan comillas.

Sort command

Te permite mostrar los campos de la forma ordenada, acendiente o descendetne. Y se ordenan por :  
- Alfabetico  
- Numerico  
- Combinaciones