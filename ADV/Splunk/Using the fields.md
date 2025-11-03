## 1. Using the fields side bar

La barra de campos, contiene todos los cambios que fueron extraídos en la búsqueda. Y se divide en:

- Selected fields:  son los campos que mas importancia tienen, se muestran en la parte superior de la lista y en la parte de abajo de cada evento. Y como se meciono antes los campos default que siempre se muestran son host, source y sourcetype.   
- Interesting fields: esto son campos que tienen valores en al menos un 20% de los eventos, ya que no todos van a tener un action, pero si al menos un 20% los tiene se muestra.

En estos valores si tiene una letra "a" minúscula antes, es un valor string, y si tiene el símbolo de hash "#" es un numeral.

Si seleccionan un campo va a tener una lista de valores del campo, un conteo de estos valores y el porcentaje de eventos que tienen este valor.

Y al dar click en estos se puede añadir a la búsqueda.

## 2. Fields in Search Queries

Los nombres de los campos son sesibles a las mayúsculas, y los valores no.

se puede usar el = y != en todos los datos. y el >, >=, < y <= solo en valores numericos

Con el IN se pueden añadir multiples opciones en vez de usar el OR muchas veces

Con el comando fields añadimos un campo, con -fields lo quitamos

Con rename, tenemos la capacidad de cambiar el nombre de los campos que aparecen en la busqueda

## 3. Fields in Search Results

comando eval se usa para calcular y manipular el valor de los campos. Y los resultados de este se escriben en un campo temporal nuevo. Como hacer cálculos y ese tipo de datos.

comando erex y rex extraen campos de los datos usando regex

el erex es como el extractor de campos automatico, le das una muestra de los datos y splunk trata de extraer lo que necesitas es bueno para búsquedas rápidas pero no es infalible

el rex permites usar regex llamadas capture groups para extraer los valores en el tiempo de búsqueda

## 4. Enriching data with knowldge objects