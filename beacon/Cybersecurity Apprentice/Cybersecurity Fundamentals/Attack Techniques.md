# Cyberattack Techniques

## Business Email Compromise (BEC)

Es uno de los tipos de ataques mas comunes que las organizaciones enfrentan todos los días. BEC le cuesta a las organizaciones tres veces mas que cualquier otro tipo de ciberataque. 

Spam: Es el proceso of mandar contenido no solicitado a endpoints objetivos, se hace por email. 
Spim: Sigue el mismo proceso del Spam, pero el medio es diferente, siendo este por mensajeria instantanea tipo WhatsApp, Telegram, etc. 
Vishing: Es un ataque que se caracteriza por ser con medios de audio, ya sea una llamada con una persona o una IA. 

## Phishing Attacks

Se confunde muchas veces al Spam y el Phishing, pero no son lo mismo, ya que a diferencia del Spam, los ataques de phishing son mas sofisticados y dificiles de idenfiticar. 

Spear Phishing: Es un ataque cibernetico dirigido a un individuo o grupo especifico, utilizando tecnicas de ingeneria social para engañar a la victima y obtener informacion confidencial, instalar malware o realizar otras acciones. 
Whaling: Tipo de spear phishing que se centra en atacar altos directivos de una organizacion. 
Whatering hole: Este se caracteriza por comprometer sitios web que son muy visitados por la victima o por crear sitios identicos a los objetivos con el fin de obtner informacion. 
Pharming: Este ataque redirige trafico legitimo de un sitio web a uno falso, normalmente modificando el archivo host local de un endpoint o comprometiendo un servidor DNS (DNS poisoning)

## Bots and Botnets

Esto son  notoriamente dificiles de detectar y defender para una organizacion, usando sistemas anti-malware tradicionales. 

Bots: son endpoints individuales que han sido infectados con malware que permite al atacante tomar el control del endpoint comprometido. 
Botnets: es una red de bots que trabajan en conjunto bajo el control de ciertos atacantes usando numerosos servidores. 
Instancias de bots y botnets: En una botnet, el malware avanzado trabaja en conjunto hacia un objetivo en comun, y cada bot aumenta el poder y la capacidad destructiva de la red en su conjunto. La comunicacion entre los bots individuales y al red de bots mas grande a traves de servidores C2 proporciona resiliencia a la red. 
Flexibility and Ability: Con flexibilidad y habilidad para evadir defensas, las redes de bots presentan una amenaza para la organizacion.  

### Retos de deshabilitar una botnet

Para desactivar una botnet es vital separar a los bots (endpoints infectados) del cerebro (C2 server). Y se deben seguir los siguientes pasos: 

1. Deshabilitar el acceso a internet
2. Monitorear la actividad en la red local
3. Remover dispositivos infectados y software
4. Instalar los parches de seguridad mas recientes

## DDoS attacks

Un ataque DDoS es un tipo de ciberataque en el que se envían volúmenes extremadamente altos de tráfico de red, como paquetes, datos o transacciones, a la red de la víctima objetivo para que su red y sus sistemas (como un sitio web de comercio electrónico u otra aplicación web) dejen de estar disponibles o se vuelvan inutilizables.

Y se pueden usar siguiendo las siguientes tecnicas: 

Usar bots: Una red de bots DDoS utiliza bots como parte de un ataque DDoS, saturando un servidor o red objetivo con tráfico procedente de un gran número de bots. En este tipo de ataques, los propios bots no son el objetivo del ataque. En su lugar, los bots se utilizan para saturar con tráfico algún otro objetivo remoto. El atacante aprovecha la enorme escala de la red de bots para generar tráfico que satura los recursos de red y servidor del objetivo.

Ataques de fuerza bruta: A diferencia de otros tipos de ciberataques, un ataque DDoS no suele emplear un enfoque prolongado y sigiloso. En cambio, un ataque DDoS suele adoptar la forma de un ataque de fuerza bruta muy visible, cuyo objetivo es causar rápidamente daños a la red y la infraestructura de sistemas de la víctima, así como a su negocio y reputación.

Objetivo: Los ataques DDoS suelen dirigirse contra organizaciones específicas por motivos personales o políticos, o para extorsionar con el pago de un rescate a cambio de detener el ataque DDoS. Los ataques DDoS suelen ser utilizados por hacktivistas para promover o protestar por una agenda política o causa social concreta. Los ataques DDoS también pueden utilizarse con fines de extorsión criminal para obtener un cuantioso rescate a cambio de poner fin al ataque.


