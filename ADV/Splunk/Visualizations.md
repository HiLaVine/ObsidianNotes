## Formatting Commands

Comando fields, te permite agregar o quitar campos del resultado de una búsqueda. Esto sirve para limitar la información y hacer una búsqueda mas rápida

ejemplo

| field product_name Price ==> solo mostrara los dos campos indicados   
| field - product_name Price ==> muetra todo menos los campos indicados nota: si el -esta pegado se quita solo ese campo

Comando table, es similar a field en que se pueden especificar campos para mantener en los resultados. La diferencia es que este es un comando de transformación que retiene los datos en un modo tabular. Este se puede combinar con fields, para que la búsqueda sea mucho mas eficiente y no te regrese toda la info posible, solo lo que pides.

Comando dedup para remover eventos duplicados de los resultados que comparten valores en común.

Comando addtotal, va a sumar y crear una columna de total.

Comando fieldformat, se usa si quieres un formato especifico para tus valores sin hacer cambios en los datos crudos

## Visualizing Data

Cada búsqueda que regresa valores estadísticas pueden ser visto como una grafica.

### comandos de transformación

Estos comandos ordenan los resultados de las búsquedas en tablas de datos que pueden ser usadas para propósitos estadisticos y se usan para transformar los datos en objetos visuales.

top: encuentra los valores mas comunes en un set de resultados

rare: muestra los valores menos comunes en un set de datos

stats: para producir estadísticas de una búsqueda, usamos este comando. Este tiene funciones comunes como count, distinct count, sum, average, min, max, list, values.

chart: puede tomar dos clausulas, over and by. Las clausulas de over dicen cual campo queremos en el eje x

timechart:

trendline:

### Comandos clausula

estas pueden ser usados con los comandos para hacer modificaciones en las columnas o para mostrar o no mostrar info

## Generating maps

Choropleth maps

es un tipo de mapa que te permite ver tu información con una visión geográfica, te permite usar shading para mostrar métricas

## Single Value Visualization

## visual formating