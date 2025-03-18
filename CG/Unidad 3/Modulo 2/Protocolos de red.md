Anki => SI
Son un conjunto de reglas usadas por dos o mas dispositivos en una red para describir el orden de entrega y estructura de los datos. 

Básicamente son como instrucciones que vienen en el paquete de datos.   

*Address Resolution Protocol (ARP)

Es un protocolo de red usado para determinar la dirección MAC del siguiente router o dispositivo en el path. 



## Categorías de los protocolos de red

Se pueden dividir en tres categorías, de comunicación, de gestión y de seguridad. 

### Protocolos de comunicación

Estos rigen el intercambio de información en al transmisión de redes. Determinan como se transmiten los datos y el momento de comunicación y la forma de recuperar datos perdidos durante el trayecto. 

Transsmission Crontrol Protocol (TCP)

Es un protocolo de comunicación en internet que permite a dos dispositivos crear una conexión para poder enviar datos. (capa de transporte TCP/IP) Este utiliza un proceso de tres pasos:
1. El dispositivo envía una solicitud de sincronización (SYN) a un servidor.
2. El servidor responde con un paquete SYN/ACK para confirmar la recepción
3. El dispositivo responde con un ACK lo que establece la conexión. 

User Datagram Protocol (DNS)

Es un protocolo sin conexión que no establece un enlace entre dispositivos, ya que una vez recibe la solicitud, envia toda la información. Esto lo hace menos confiable que TCP pero si mucho mas rápido y se necesita un mejor control del manejo de los datos (capa de transporte)

HyperText Transfer Protocol (HTTP)

Es un protocolo de red (capa de aplicación) que proporciona un método seguro de comunicación entre cliente y un servidor web. 

Domain Name System (DNS)

Un protocolo de red que traduce los dominios de internet a direcciones ip. 

### Protocolos de gestión

Se utilizan para monitorear y administar la actividad en red (se usan para el prtg)

Simple Network Managment Protocol (SNMP)

Se utiliza para monitorear y gestionar los dispositivos en una red. (esta en la capa de aplicacion) 

Esta en el puerto 161/UDP para solicitudes y 162/UDP para traps SNMP

Internet Control Message Protocol (ICMP)

Es utilizado para comprobar la disponibilidad y latencia de dispositivos en la red. 

Se usa con el ping y tracert. 

### Protocolos de seguridad

Garantizan qu elos datos se envíen y reciban de forma segura a través de una red. Usan algoritmos de cifrado para proteger los datos durante su transmisión. 

Secure File Transfer Protocol (SFTP)

Es un protocolo seguro para la transferencia de datos que funciona sobre el SSH(Secure Shell). Usa el mismo puerto que el SSH 22