Las suites de protocolos surgen debido la existencia de muchos fabricantes de dispositivos, lo que implica que ciertos protocolos son propiedad de ciertos fabricantes y que solo se pueden utilizar bajo licencia. 

Existen otros protocolos que pertenecen que pertenecen a estándares abiertos, lo que permite una comunicación entre dispositivos de distintos proveedores. 

Un ejemplo seria la interacción entre un servidor web y un navegador, donde se ven usados diferentes protocolos. Que son los siguientes: 

| Capa             | Protocolo                                            | Descripción                                                                                                                                                                                                          |
| ---------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aplicación (TCP) | Protocolo de Transferencia de hipertexto (HTTP - 80) | Define el contenido y el formato de las respuestas intercambiadas entre cliente y servid                                                                                                                             |
| Transporte (TCP) | Protocolo de control de transmición (TCP)            | Divide los mensajes HTTP en partes mas pequeñas llamadas segmentos para enviarlas a su desti                                                                                                                         |
| Internet         | Protocolo de internet (IP)                           | Es el responsable de tomar los segmentos TCP encapsular los paquetes,  asignar las direcciones y escoger la mejor ruta hacia su host dest                                                                            |
| Acceso de red    | Ethernet                                          Administran el enlace de datos tomando los paquetes IP y los formatean para enviarlos por los medios. Y también se encargan de administrar los  medios físicos viendo como se envía de dispositivos a dispositivo.  ivo.  |

## Modelos básicos de Networking

Tenemos dos modelos básicos, por un lado los de protocolos y por el otro los de referencia. 

El modelo de protocolo proporciona un modelo que coincide fielmente con la estructura de una suite de protocolos en particular. Representa típicamente toda la funcionalidad requerida para que funcione la red humana con la red de datos.

Y un ejemplo de este es el modelo TCP/IP ya que describe las funciones que se producen en cada capa de los protocolos dentro del conjunto TCP/IP. 

Por otro lado un modelo de referencia proporciona una referencia común para mantener consistencia en todos los protocolos y servicios de red. Y tiene como propósito principal asistir en la compresión mas clara de las funciones y procesos involucrados y el mas conocido es el Modelo OSI (Open Systems Interconnection). 

## Modelo TCP/IP

Este es un modelo de protocolo conformado en capas, y describen un stack de protocolos en especifico de proveedor pero este es un protocolo de estándar abierto. 

![[Pasted image 20250819195704.png]]
Y sigue el siguiente proceso: 

1. Se crean los datos en la capa de aplicación. 
2. Bajan a la siguiente capa donde se encapsulan y segmentan los datos. 
3. Luego se generan datos sobre el medio y se transportan los datos. 
4. Se reciben los datos.
5. Se des-encapsulan y rearman los datos en el host destino. 
6. Y por ultimo se pasan los datos a la capa de aplicación.

La forma que adopta una sección de datos en cualquier capa se denomina PDU (Unidad de datos de protocolo)

Y cada capa hace lo siguiente: 

* Capa de aplicación: Representan datos para el usuario más el control de codificación y diálogo. 
* Capa de transporte: Admite la comunicación entre dispositivos de distintas redes. (su pdu se denomina Segmento para TCP y Datagrama para UDP)
* Capa de Internet: Determina la mejor ruta a través de la red. (su pdu se denomina Paquete)
* Capa de Acceso a la red: Controla los dispositivos del Hardware y los medios que forman la red. (su pdu se denomina trama)

![[Pasted image 20250819200930.png]]