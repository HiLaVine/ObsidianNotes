tcpdump es un analizador de paquetes de red de línea de comandos, es popular por ser ligero y usar la biblioteca de código abierto libpcap. 

Interpretacion de la salida: 

tcpdump imprime la salida del comando como los paquetes detectados en la liena de comandos y, opcionalmente, es un archivo de registro. 

![[Pasted image 20250325113001.png]]
Parte de la información que se recibe de una captura de paquetes es: 

- **Marca de tiempo**: la salida comienza con la marca de tiempo, en el formato de horas, minutos, segundos y fracciones de segundo. 
    
- **IP de origen**: el origen del paquete es proporcionado por su dirección IP de origen.
    
- **Puerto de origen**: el número de puerto de donde se originó el paquete.
    
- **IP de destino**: la dirección IP de destino es el lugar al que se transmite el paquete.
    
- **Puerto de destino**: el número de puerto del lugar al que se transmite el paquete.