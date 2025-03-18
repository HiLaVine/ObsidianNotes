Anki => NO
## Network Address Translation (NAT)

Es un tipo de red en la que un router o firewall traduce direcciones IP privadas en una única dirección IP pública para que los dispositivos de una red interna puedan acceder a internet o comunicarse con otras redes. 

## Dynamic Host Configuration Protocol (DHCP)

El protocolo de configuración dinámica de host (DHCP) es un protocolo de gestion. 

Este es un protocolo de la capa de aplicación utilizado para configurar dispositivos de manera automática dentro de una red. Asignando automáticamente direcciones ip y otros parámetros de configuración a los dispositivos en red. 

Este protocolo opera en el puerto 67 UDP para servidor y 68 UDP para cliente. 

## Address Resolution Protocol (ARP)

Es un protocolo de comunicación que asocia una dirección IP a una dirección MAC. Este protocolo es capaz de convertir las direcciones IP en direcciones MAC. 
**el ARP garantiza que un dispositivo siempre pueda encontrar la dirección MAC correcta**, incluso si la dirección IP cambia.

Trabaja en capa 2 y 3. 

## Telnet 

Es un protocolo de capa de aplicacion que permite que un dispositivo se comunique con otro equipo o servidor. Telnet envia información en texto claro. Este no se puede utilizar para conectarse a dispositivos locales o remotos y utiliza el puerto TCP 23. Mayormente obsoleto. 

## Secure Shell (SSH)

Se utiliza para crear una conexión segura con un sistema remoto. Este proporciona una alternativa para la autenticacion segura y la comunicacion cifrada. Opera sobre el puerto TCP 22 y es mas seguro que telnet.  

## Post Office Protocol (POP)

Es un protocolo de la capa de aplicacion (4 tcp/ip) Este**protocolo de correo electrónico** que permite a los usuarios **descargar correos desde un servidor de correo a su dispositivo local**. Una vez descargados, los correos generalmente se eliminan del servidor.

- **POP2 (1984)** → Usaba autenticación en texto plano y funcionaba sobre Telnet.
- **POP3 (1988 - Actual)** → **Versión más usada hoy en día**, con soporte para **autenticación segura** y acceso por SSL/TLS.

|**Protocolo**|**Puerto estándar**|**Cifrado**|
|---|---|---|
|**POP3**|110|❌ No cifrado|
|**POP3S**|995|✅ SSL/TLS|

💡 **POP3S** (POP3 con SSL/TLS) es más seguro y se recomienda para conexiones cifradas.


## Internet Messagge Access Protocol (IMAP)

Es un **protocolo de correo electrónico** que permite a los usuarios **acceder a sus correos electrónicos directamente en el servidor sin necesidad de descargarlos**. 

A diferencia de **POP3**, IMAP **sincroniza los correos entre el servidor y todos los dispositivos**, lo que lo hace ideal para quienes revisan su correo en **varios dispositivos (PC, teléfono, tablet, etc.)**.

**¿Qué puertos usa IMAP?**

|**Protocolo**|**Puerto estándar**|**Cifrado**|
|---|---|---|
|**IMAP**|143|❌ No cifrado|
|**IMAPS**|993|✅ SSL/TLS|

💡 **IMAPS (IMAP con SSL/TLS)** es la versión segura y cifrada, recomendada para proteger la información.

## Simple Mail Transfer Protocol (SMTP)

Se utiliza para transmitir y enrutar correos electronicos desde el remitente hast ala dirrecion del destinatario. Funciona con el software Message Transfer Agent (MTA) que consulta los servidores de DNS para obtener las ip correspondientes a las direcciones de correo electronico. 

Usa el puerto 25 para no cifrados y el 587 para utilizar TLS para los cifrados. 

|**Protocolo**|**Puerto**|
|---|---|
|DHCP|Puerto UDP 67 (servidores)<br><br>Puerto UDP 68 (clientes)|
|ARP|Ninguno|
|Telnet|Puerto TCP 23|
|SSH|Puerto TCP 22|
|POP3|Puerto TCP/UDP 110 (sin cifrar)<br><br>Puerto TCP/UDP 995 (cifrado, SSL/TSL)|
|IMAP|Puerto TCP 143 (sin cifrar)<br><br>Puerto TCP 993 (cifrado, SSL/TSL)|
|SMTP|Puerto TCP/UDP 25 (admite cifrado TSL)<br><br>Puerto TCP/UDP 587 (cifrado, TSL)|

## Protocolos Inalámbricos

IEEE 802.11 (WIFI)

Un conjunto de estándares que definen la comunicación de LAN'S inalámbricas. 

WIFI Protected Access (WPA)

Un protocolo de seguridad inalámbrico para dispositivos que se conectan a internet. 

