# Modern Endpoint Security

## ¿Qué es un Endpoint?

Un endpoint es un dispositivo de computo remoto que se comunica con una red a la que esta conectado. Esto incluye laptops, moviles, servidores, estaciones de trabajo, pc de escritorio, dispositivos IoT, y estos son puntos clave para la entrada de los cibercriminales. 

### Objetivos comunes en los endpoints

Los endpoints es donde los atacantes ejecutan el código y explotan vulnerabilidades, y estas contienen assets para encriptar, extraer o aprovechar. Los endpoints se estan volviendo cada vez mas suceptibles, a los ciberataques, debido a que las fuerzas de trabajo de las organizaciones cada vez se vuelven mas moviles, y les permiten conectar a los recursos internos desde endpoints off-premise a lo largo del mundo. 

Y los objetivos principales son los siguientes:

* Usarlo como un punto de entrada/salida para obtener acceso a informacion de gran valor en la red de la organizacion.
* Obtener informacion desde el endpoint para filtrarla o hacer algun ataque de ransom, o simplemente causar daños al proceso de trabajo.
* Tomar control del equipo y usarlo como un botnet para ejecutar un DoS o un DDoS.

## Endpoint Detection and Response (EDR)

Esto se refiere a una herrmienta usada para detectar e investigar amenazas en los endpoints. EDR provee deteccion, analisis, investigacion y capacidades de respuesta. 

* Deteccion: Las herramientas EDR supervisan los eventos generados por los agentes de los endpoints para buscar actividades sospechosas. Y las alertas que crean ayudan a los analistas a identificar, investigar y solucionar problemas. Y tienen las siguientes capacidades de deteccion:
    * Agregacion de datos de los endpoints.
    * Análisis de malware.
    * Análisis de comportamiento, o la capacidad de conectar con la cadena de eventos para detectar comportamientos maliciosos.
    * Correlacion y enriquecimiento de datos.
    * Correlación de alertas relacionadas en incidentes.
    * Priorizacion basada en la confianza y la gravedad de los incidentes.

* Investigacion: Las herramientas EDR, recolectan los datos de actividad sospechosa y enriquecen esa informacion con otra informacion contextual de eventos correlacionados. Y tiene las siguientes capacidades:
    * Concultar actividad a muchas herramientas de ciberseguridad.
    * Investigar herramientas que proveen en flujo de trabajo integrado con sistemas de tickets.
    * Las herramientas de visualización de cadenas de ataques de clic permiten a los investigadores pivotar.

* Respuesta: Es fundamental para acortar los tiempos de respuesta de los equipos de respuesta a incidentes gracias a sus funciones:
    * Análisis automatizado e integrado con un entorno aislado (sandbox).
    * Corrección, incluyendo aislamiento de la red, cuarentena de archivos, eliminación de archivos, recreación de imágenes, eliminación de procesos y bloqueo de       comportamientos.
    * Flujos de trabajo de respuesta y corrección automatizados basados en políticas o guías predefinidas.

## Extended Detection and Response

XDR es una evolución del EDR, es una nueva herramienta para la deteccion y respuesta a amenazas. La X representa cualquier fuente de datos, como sensores de red, nube o endpoints. 

### Evolucion del EDR

Las herramientas tradicionales de EDR solo se centran en los datos del endpoint, lo que provee una vision limitada en las sospehcas de amenaza. Lo que resulta en detecciones fallidas, muchos falsos positivos y investigaciones mas largas. Estas deficiencias agravan los retos de los equipos de seguridad, aparte de la sobrecarga de eventos, escasez de personal cualificado, herramientas limitadas, falta de integracion y falta de tiempo. 

Los sistemas XDR usan heuristicas, analisis, modelado y automatizacion para combinar y obtener información de estas fuentes, lo que aumenta la visibilidad y la productividad de la seguridad en comparacion con otras herramientas. Lo que simplifica el proceso de investigacion, reduciendo el tiempo para descubrir, buscar, investigar, y responder a las amenazas.

### ¿Por qué usar XDR?

Debido a los diferentes ataques y debilidades de los sistemas, los ciberataques modernos se han dirigido tanto a los sistemas como a los usuarios finales, ademas de que las herramientas comunes pueden eludirse con exploits de PowerShell. 

Ademas de que EDR y XDR pueden dar información exacta como: 

* ¿Cuando paso el ataque?
* ¿Que metodos uso?
* ¿Porque el ataque fue exitoso?
* ¿Que tipo de ataque fue?
* ¿Que o quien fue afectado (sistemas u organizaciones)?

## Endpoint Security

Endpoint Security, describe las herramientas, productos, y tecnicas diseñadas para proteger a los equipos de los usuarios y que que fortalece la seguridad de accesos individuales a la red y datos sensibles de una organizacion. 

### ¿Por qué es importante?

Debido al creciente uso de dispositivos moviles y su uso por parte de los trabajadores, el numero de vulnerabilidades en las redes de las organizaciones crece.  Por lo que las organizaciones deben fortalecer estos puntos debiles para protegerse de los ciberataques. 

### Endpoint proteccion Platform

El termino "Endpoint Security" es casi un sinonimo de "Endpoint Proteccion Platform" o EPP. Esta se coloca en los endpoints y los protege de los ciberataques basado en combatir el malware mas avanzado. 

* EPP: usa muchas tecnicas de prevencion, como el analisis de estadisticas para evaluar el malware potencial basado en la inspeccion de archivos, heuristicas, y comportamiento para evaluar un archivo malicioso basado en sus funciones.
* EDR: Nace como apoyo para las herramientas EPP, y permiten a los equipos de seguridad investigar y mitigar las amenazas que sus herramientas pasan por alto. 

### Capacidades clave de los EPP

Los mejores EPP ofrecen una gestion en la nube, para poder mantener el monitoreo constante y los problemas se resuelvan automaticamente sin importar la red a la que el endpoint este conectado. 

Y sus capacidades son: 

* Bloquear malware conocido y desconocido.
* Deteccion precisa.
* Analisis de comportamiento.
* Gestion efectiva y facil.

## Endpoint Security Strategies

1. Sistemas de seguridad modernos para endpoints basados en comportamiento y no en firmas.
2. Empresas de seguridad de endpoints que combinen EPP y EDR para mejorar el servicio.
3. Seguridad integral de endpoints ofreciendo soluciones de seguridad poderosas y completas como XDR.
4. Seguridad de endpoints avanzada que previene el malware conocido y desconocido y que ayuda a los teams de seguridad.

## User and Entity Behavior Analytics

Conocido como UEBA o UBA es un tipo de solucion de ciberseguridad que detecta amenazas medienta la identificacion de actividades que se desvian de una linea normal. 

UEBA monitorea y detecta actividad inusual en las redes de computadoras, incluyendo accesos no autorizados o comportamiento sospechoso. 

### Diferencias entre UEBA y NTA 

* Log-Centric solutions: Las soluciones UEBA suelen estar integradas en productos de seguridad tradicionales, como los agentes de seguridad de acceso a la nube y los sistemas de administración y gobernanza de identidades. Las soluciones UEBA utilizan datos históricos y en tiempo real, así como el aprendizaje automático, para desarrollar una línea de base de actividad estándar de los usuarios de la red y otras entidades (por ejemplo, hosts, aplicaciones, repositorios de datos, tráfico de red).

Una vez establecida esta referencia, las soluciones UEBA aplican métodos analíticos (por ejemplo, estadísticas simples, comparación de patrones, reglas que aprovechan las firmas) para buscar anomalías en los patrones de tráfico que indiquen actividades potencialmente sospechosas o maliciosas. Para que las soluciones UEBA realicen análisis de comportamiento de forma eficaz, la empresa debe disponer primero de un conjunto de datos sólido e integrado para las herramientas de aprendizaje automático.

* Network-Centric Solutions: Las soluciones NTA utilizan aprendizaje automático, análisis avanzados y detección basada en reglas para supervisar y analizar todos los registros de tráfico y flujo en las redes empresariales. Las soluciones NTA utilizan esta información para identificar posibles ataques, abusos internos, actividades sospechosas y malware. Estas soluciones supervisan y analizan todo el tráfico norte-sur a través del perímetro de la empresa y todas las comunicaciones este-oeste desde los sensores de red.


