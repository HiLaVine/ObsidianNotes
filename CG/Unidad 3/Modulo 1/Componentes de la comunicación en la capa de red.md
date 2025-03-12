Operaciones de la capa de red.

Las funciones de esta capa son organizar la dirección y la entrega de paquetes de datos a través de la red e internet desde el dispositivo host al destino.

Dirige paquetes de un enrutador a otro a traves de internet basado en su direccion ip de la red destino.

Esta ip esta dentro del encabezado de cada paquete de datos.

Estos paquetes tiene una ip que se denomina paquete up o datagrama. El router utiliza la direccion ip para enrutar paqutes de una red a otra basado en la info contenida del encabezado ip.

Formato de un paquete IPv4

El tamaño del paquete va de 20 a 65,536 bytes.

Este tiene dos secciones el encabezado y los datos:

  - El tamaño del encabezado o header Ip oscila entre 20 y 60 bytes. Incluye la información de enrutamiento ip que los dispositivos usan para para dirigir el paquete.

  - La longitud de la sección de dato sde un paquete IPv4 puede variar según el tamaño de la información enviada pero el maximo qu epuede contener es de 65,536 bytes.

Hay 13 campos dentro del encabezado de un paquete IPv4:

- **Versión:** el primer encabezado de 4 bits indica a los dispositivos receptores qué protocolo está utilizando el paquete. El paquete utilizado en la ilustración anterior es un paquete IPv4.
    
- **Longitud del encabezado IP (HLEN):** HLEN es la longitud del encabezado del paquete. Este valor indica dónde termina el encabezado del paquete y comienza el segmento de datos. 
    
- **Tipo de servicio (ToS):** los routers priorizan los paquetes a entregar con el fin de mantener la calidad del servicio en la red. El campo ToS proporciona esta información al router.
    
- **Longitud total:** este campo comunica la longitud total de todo el paquete IP, incluidos el encabezado y los datos. El tamaño máximo de un paquete IPv4 es de 65.535 bytes.
    
- **Identificación:** si el paquete IPv4 es superior a 65 535 bytes, se divide o fragmenta en paquetes IP más pequeños. El campo de identificación proporciona un identificador único para todos los fragmentos del paquete IP original para que puedan volver a ensamblarse cuando lleguen a su destino. 
    
- **Indicadores:** este campo proporciona al dispositivo de enrutamiento más información sobre si el paquete original se fragmentó y si hay más fragmentos en tránsito.
    
- **Desplazamiento de fragmentación:** el campo de desplazamiento de fragmento indica a los dispositivos de enrutamiento a qué parte del paquete original pertenece el fragmento.
    
- **Período de vida (TTL):** evita que los routers reenvíen los paquetes de datos de manera indefinida. Contiene un contador que determina la fuente. El contador disminuye de a uno, a medida que pasa por cada router. Cuando el contador TTL llega a cero, el router descartará el paquete y enviará al emisor un mensaje de tiempo superado ICMP. 
    
- **Protocolo:** este campo indica al dispositivo receptor qué protocolo se utilizará para el área de datos del paquete.
    
- **Suma de comprobación del encabezado:** este campo contiene una suma de comprobación que se puede usar para detectar si la cabecera IP en tránsito está dañada. Los paquetes dañados se descartan.
    
- **Dirección IP de origen:** es la dirección IPv4 del dispositivo emisor.
    
- **Dirección IP de destino:** es la dirección IPv4 del dispositivo receptor.
    
- **Opciones:** este campo permite aplicar opciones de seguridad al paquete si el valor HLEN es mayor que cinco. Además, comunica estas alternativas a los dispositivos de enrutamiento.
![[Pasted image 20250312102317.png]]

![[Pasted image 20250312102650.png]]

Elementos del ipv4 que pasan a ipv6