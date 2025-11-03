## Creating a Scheduled Reports

Un Schedule report es un reporte que corre en un intervalo de tiempo definido. Cuando un reporte corre, puede automáticamente mandar un mail o disparar acciones adicionales. También se pueden usar para alimentar dashboards para prevenir que splunk corra de forma concurrente multiples búsquedas

aparte de las configuraciones se puede usar una Schedule window solo si el reportes no tiene que empezar en un momento especifico y puede tener un delay.

Los admins pueden gestionar y añadir perbuilts de las alertas usando el manage actions

## Managing Reports

Los usuarios con el power role tienen la opción de desplegar el reportes para ellos y otros usuarios de la app. Y para desplegarlo en todas las apps se necesita tener el rol de admin

a un reporte endebido tiene acceso cualquier persona que pueda acceder a la pagina web.

## What are Alerts?

En splunk están basadas en búsquedas que corren en intervalos de tiempo predefinido o en tiempo real. Estas se notifican cuando los resultados de una búsqueda corresponden a unas condiciones definidas y se disparan cuando la búsqueda esta terminada

Una alerta puede

listar una interface  
log events  
output to lookup  
send to a telemetry endpoint  
Trigger Scripts  
Send emails  
Use a webhook  
Run a custom alert

## Creación de alertas

Primero definimos la búsqueda

Los permisos de la alerta, pueden ser privados y Shared in App. En el privado solo tu puedes acceder, editar y revisar la alerta. Y la de shared in app deja que todos los usuarios de la app puedan verla. Por defaul todos tienen acceso de lectura y los power users tienen acceso de escritura.  

existen dos tipos de alertas, el de Schedules y el de Real-time. La primera te permite establecer un rango de tiempo y una fecha para correr la búsqueda. Y las de real time permiten corren la búsqueda continua en el fondo y en cuanto las condiciones se son satisfechas lanza la alerta.

Luego se ponen las condiciones de disparo, con las que la alerta se norificara.

## Using alert actions

Aquí se colocan las acciones que llevaran a cabo las alertas una vez se notifiquen. Como ser mandadas por correo, indexarse en alguna sección, correr algún script, etc.

## Managing Alerts