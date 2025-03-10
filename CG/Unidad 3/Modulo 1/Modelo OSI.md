![[Pasted image 20250226112643.png]]

Capa 7: Capa de aplicación. 

Esta capa incluye procesos que involucran directamente al usuario cotidiano. Aquí se incluyen todos los protocolos de red que las aplicaciones de software utilizan para conectarlo a internet. 

Esta característica es la que identifica a la capa de aplicación: conexión de usuarios a través de aplicaciones y solicitudes. 

Aquí es donde se coloca el uso del navegador web, con sus protocolos de HTTP (puerto 80) y HTTPS (puerto 443) para enviar y recibir información del servidor. La aplicación del correo electrónico que utiliza el SMTP (simple mail transfer protocol puerto 587). Y también el uso del protocolo de sistema de nombres de dominio (DNS - Domain Name System puerto 53) que traduce el nombre de las ip a los nombres de dominio. 

Capa 6: Capa de presentación.

En esta capa se hace la traducción de datos y el cifrado para la red. Aquí se agrega y reemplaza datos con formatos que pueden ser entendidos por las aplicaciones en los sistemas de envío y recepción. 

Los procesos de la capa de presentación requieren el uso de un formato estandarizado. 

Algunas funciones de formateo que se producen en la capa 6 incluyen el cifrado, compresión y confirmación de que el conjunto de caracteres puede ser interpretado en el sistema receptor. Un ejemplo de cifrado es el SSL (Secure Sockets Layer) que cifra los datos entre los servidores web y los navegadores como parte de sitios con HTTPS. 

Capa 5: Capa de sesión.

Una sesión indica cuando se establece una conexión entre dos dispositivos. Una sesión abierta permite que los dispositivos se comuniquen entre sí. 
El objetivo de los protocolos de la capa de sesión es mantener la sesión abierta mientras se transfieren los datos y cerrarla una vez terminen. 

Esta capa también es responsable de actividades como la autenticación, reconexión y establecimiento de puntos de control durante una transferencia de datos. Estos puntos de control aseguran que si la conexión se ve interrumpida se guarde hasta donde se quedo y cuando se retome la conexión no se empiece desde cero la transmisión. 

Las sesiones incluyen una solicitud y respuesta entre aplicaciones, esta capa responde a solicitudes de servicio de procesos de la capa 6 y envía dichas solicitudes a la capa 4. 

Capa 4: Capa de transporte.

La capa de transporte es la responsable de enviar datos entres dispositivos. Aquí se maneja la velocidad y el flujo de transferencia y divide los datos en segmentos mas pequeños para facilitar el envió. 

Para que se pueda procesar en la capa 5, estos segmentos tiene que volverse a ensamblar en su destino y el tipo de protocolo que se uso, ya sea TCP o UDP.

Capa 3: Capa de red.

Supervisa la recepción de los paquetes desde la capa 2 y las entrega al destino previsto. Estos paquetes incluyen direcciones IP que indican a los routers donde enviarlos y se enrutan desde la red de envio hacia la red de recepcion. 

Capa 2: Capa de enlace de datos. 

Organiza el envió de datos y la recepción de paquetes de datos dentro de una sola red. Esta capa incluye switches en la red local y las tarjetas de interfaz de red en los protocolos locales. 

En la capa de enlace de datos se utilizan protocolos como el protocolo de control de red (NCP - Network Control Protocol), el control de enlace de datos de alto nivel (HDLC - High-Level Data Link Control) y el protocolo de control de enlace de datos sincrónico (SDLC - Synchronous Data Link Control).

Capa 1: Capa física 

Como su nombre lo indica, la capa física corresponde al hardware físico utilizado en la transmisión de la red. Los hubs, los módems y el cableado que los conecta se consideran parte de esta capa. Para viajar a través de un cable Ethernet o coaxial, un paquete de datos debe ser traducido en una secuencia de ceros y unos, que se envía a través de los cables y conexiones físicas, se recibe y, luego, pasa a los niveles superiores del modelo OSI.