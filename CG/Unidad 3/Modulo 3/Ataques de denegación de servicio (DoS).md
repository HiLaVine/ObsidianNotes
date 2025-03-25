Este tipo de ataque va contra una red o servidor y lo inunda con tráfico de red. Un ataque de denegación de servicio o ataque DoS interrumpe o altera las operaciones al sobrecargar la red de una empresa. 

Su objetivo es enviar tanta información a un dispositivo de red hasta que falle o no pueda responder a usuarios legitimos. 

Un DDoS (Distributed denial of service attack) es un ataque DoS que usa varios dispositivos o servidores en diferetnes lugares para inundar la red víctima de tráfico no deseado. Al usar muchos dispositivos, es mas probable que el trafico sobrecargue el servidor destino. 

**icmp**(internet control message protocol): es un protocolo de internet usado por los dispositivos para contarse unos a los otros acerca de los errores de transmision de información a travez de la red.  

Ataques DoS cuyo objetivo es la banda ancha:

- Ataque de inundación sincronizada (SYN flood attack): Simula una conexión TCP e inunda el servidor con paquetes SYN. Lo que impide al servidor funcionar bien ya que se ve forzado a responder a todas las peticiones, llevándolo al colapso.  
- ICMP flood attack: se lleva a cabo cuando el agente de amenaza manda repetidos paquetes ICMP a la red del servidor. Lo qu obliga al servidor a responder, lo que agota el ancho de banda al ya no poder pasar ni las solicitudes ni las respuestas. 
- Ping of death: Consiste en saturar al servidor enviando un ping mayor a los 65 KB, pero fragmentado, para que este al reconstruirlo sea incapaz por que sobrepasa el tamaño máximo para este tipo de paquete. 