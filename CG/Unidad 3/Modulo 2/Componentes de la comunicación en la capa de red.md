Operaciones de la capa de red.

Las funciones de esta capa son organizar la direccion y la entrega de paquetes de datos a traves de la red e internet desde el dispositivo host al destino.

Dirige paquetes de un enrutador a otro a traves de internet basado en su direccion ip de la red destino.

Esta ip esta dentro del encabezado de cada paquete de datos.

Estos paquetes tiene una ip que se denomina paquete up o datagrama. El router utiliza la direccion ip para enrutar paqutes de una red a otra basado en la info contenida del encabezado ip.

Formato de un paquete IPv4

El tamaño del paquete va de 20 a 65,536 bytes.

Este tiene dos secciones el encabezado y los datos:

  - El tamaño del encabezado o header Ip oscila entre 20 y 60 bytes. Incluye la información de enrutamiento ip que los dispositivos usan para para dirigir el paquete.

  - La longitud de la sección de dato sde un paquete IPv4 puede variar según el tamaño de la información enviada pero el maximo qu epuede contener es de 65,536 bytes.

El header tiene 13 campos que representan lo siguiente: