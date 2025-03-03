Es un framework usado para visualizar como los datos son organizados y transmitidos en una red. 

Este modelo es también conocido como protocolo de control de transmisión y protocolo de internet. 

Este es el modelo estándar usado para la comunicación en red. 

## TCP (Transmission Control Protocol)

Es un protocolo de comunicación en internet que permite que dos dispositivos hagan una conexión y puedan enviar y recibir datos. 

Este incluye instrucciones para organizar datos y enviarlos por la red. 

## IP (Internet Protocol)

Un conjunto de estándares usados para enrutar y direccionar paquetes de datos entre dispositivos de una red. 

Aquí se incluye la dirección ip. 

## Puerto

Es una ubicación de software que organiza el envió y recibimiento de paquetes de datos entre dispositivos de una red. 

Estos dividen a la red en segmentos basado en los servicios que prestan. 

Y los puertos comunes son los siguientes:

- Puerto 25: Email (protocolo SMTP simple mail transfer protocol). Aunque el puerto estándar es el 587 
- Puerto 443: HTTPS (Secure internet communication).
- Puerto 80: HTTP (internet communication).
- Puerto 20: Protocolo FTP (File Transfer Protocol) y se usa para transferencia de archivos grandes.

## Capas del modelo TCP/IP

1. Capa de aplicación: Los protocolos determinan cómo interactúan los paquetes de datos como los dispositivos receptores. Las funciones organizadas aquí son las de transferencia de archivos y servicios de correo. 
	- Protocolo de transferencia de hipertexto (HTTP)
	- Protocolo simple de transferencia de correo (SMTP)
	- Secure Shell o shell seguro (SSH)
	- Protocolo de transferencia de archivos (FTP)
	- Sistema de nombres de dominio (DNS)
2. Capa de transporte: Incluye los protocolos que controlan el flujo del tráfico en una red. Estos protocolos permiten o niegan la comunicación con otros dispositivos e incluyen información del estado de la conexión. Aquí también se controlan errores, que garantiza que los datos fluyan sin problemas. 
	- Protocolo de control de transmisión (TCP): Garantiza que los datos se transmitan de forma segura al sericio de destino. Contiene el numero de puerto del servicio del destino previsto que reside en el encabezado TCP de un paquete TCP/IP.
	- Protocolo de datagramas de usuario (UDP): Las aplicaciones que no están afectadas por la confiabilidad de la transmisión usan el protocolo UDP, ay que los datos enviados no son objeto de seguimiento tan exhaustivo. 
3.  Capa de internet(capa de red): Aquí las direcciones IP se adjuntan a paquetes para indicar la ubicación del emisor y receptor. También se enfoca en cómo las redes se conectan entre sí. 
	- Protocolo de internet (IP): Envía los paquetes de datos al destino correcto y se basa en el protocolo de control de transmisión/protocolo de datagramas de usuario (TCP/UDP). 
	- Protocolo de mensajes de control de internet (ICMP): Comparte información de errores y actualización de estado de los paquetes de datos. 
4. Capa de acceso a la red(enlace de datos): Esta se ocupa de crear paquetes de datos y transmitirlos por una red. E incluye dispositivos de hardware conectados a cables físicos y switches que envían datos a su destino. 

![[Pasted image 20250219120415.png]]

## Comparación del Modelo TCP/IP con el modelo OSI

![[Pasted image 20250219121731.png]]

El modelo TCP/IP combina múltiples capas del modelo OSI. Ambos modelos comparten muchas similitudes, ya que definen estándares para las redes y dividen el proceso de comunicación de red en diferentes capas. Sin embargo, el modelo TCP/IP es una versión simplificada del modelo OSI.
