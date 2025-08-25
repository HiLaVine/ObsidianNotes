# Traditional Endpoint Security

## Anti-Malware and Antivirus

Malware prevention mas especifico, antivirus sofware ha sido uno de los principios básicos de la seguridad informatica desde principios de la década de 1980, por desgracia todo este tiempo no representa una victoria. 

### Poor "Catch Rate" Factors

Esto se refiere al porque algunas soluciones de seguridad fallan en prevenir el malware. Y se tienen dos razones: 

* Habilidad para mutar y evadir la detección: algunos malware pueden mutar o actulizarce para evadir la deteccion de sistemas tradicionales anti-malware.
* Malware avanzado y customizado: Malware avanzado incrementa la especialización al punto que el atacante diseña malware especifico al objetivo.

## Deteccion Anti-Malware Tradicional

El software anti-malware basado en firmas es uno de los mas viejos y mas comunes aproximanciones para detectar e identificar malware en endpoints. 

### Basado en firmas

Esta aproximacion requiere que los fabricantes, esten recolectando muestras de malware continuamente, creando asi las firmas, luego distribuirnas en los productos de seguridad de todos sus clientes. Y sigue el proceso:

1. Despliegue: Deplegar los softwares antivirus basados en firmas, requiere la instalacion de un motor a nivel kernel, accediendo a todos los recursos del endpoint.
2. Deteccion: Estos softwares escanean los discos duros y las memorias de los endpoints, en una fecha predefinida o en tiempo real cuando se accede al archivo.
3. Remover: Si una firma de malware conocida es detectada, el sofware hace una de las siguientes cosas:
     * Cuarentena: Aisla el archivo infectado para evitar mas contagios en el endpoint.
     * Borrar: Borra el archivo infectado.
     * Alerta: Avisa al usuario o administrador que el malware ha sido eliminado.
  
### Desventajas del basado en firmas

A pesar de que este tipo de software es muy popular, su efectividad esta limitada: 

* Respuesta de contramedida lenta: por diseño, estos tienen una contramedida reactiva, lo que significa que si el malware no esta "in the wild" estos estan practicamente ciegos y desprotegidos. Ya que este proceso de lanzar y detectar puede durar de 5 hasta 20 dias.
* Degradación notable del rendimiento: Actualizar firmas se debe hacer de forma regular y frecuentemente esto se descarga desde el fabricante al endpoint del cliente. Lo que conlleva a una degradacion del rendimiento del endpoint del cliente. 
* Amplia ventana de oportunidades de ataque: Primero hay que capturar e identificar una muestra en trafico antes de que se pueda crear una firma, luego hay que descargar e instalar en el endpoint del cliente. Lo que significa que mientras todo este proceso se lleva a cabo un atacante puede crear un malware y atacar satisfactoriamente a un endpoint.
* No se detectan nuevas variables: Millones de nuevas variantes de malware son creadas año con año, y muchas de ellas no se tiene firma hasta que atacan satisfactoriamente un endpoint.
* Facil de evadir: Las tecnicas mas avanzadas de malware como el metemorfismo o el polimorfismo toman ventaja de las debilidades inherentes de estos softwares y les permiten evadir y llevar ataques a los endpoints.

## Basado en contenedores

La proteccion basada en contenedores envuelve los procesos vulnerables en una barrerta virtual protectora mientras se estan ejecutando, si un proceso es malicioso, el contenedor lo detecta y lo cierra, evitando que dañe otros procesos o archivos legítimos en el terminal. 

### Inconvenientes del enfoque basado en contenedores

Estos tipicamente requieren una gran cantidad de recursos computacionales, y los atacantes han demostrado poder rodear o deshabilitar este tipo de proteccion. 
Tambien requieren conocimiento de como funciona lo que quieren proteger y como funcionan todas las interacciones que tienen con otros componentes de software. 
Por lo tanto, esta herramienta es util para proteger software muy común, pero no para ser una herramienta de uso general. Y hay software que no funciona bien en estos entornos lo que dificulta todo mucho mas. 

## Application Allowlisting (aplicaciones permitidas)

Este metodo de proteccion es una tecnica que es muy usada para prevenir que los usuarios corran aplicaciones no permitidas en sus endpoints, y que puedan contener malware. 

* Como funcionan: requiere un modelo de control donde las aplicaciones no permitidas para correr en el endpoint, a menos que esten de forma explicita en la politica de lista permitida. Ademas de requerir un gran esfuerzo administrativo para establecer las apps permitidas, esta funcionalidad puede ser util para reducir la superficie de ataque, pero no es un enfoque integral para la seguridad de los endpoints.
* Desventajas: Las nuevas tecnologias como la nube, bring your own device(BYOD)/bring your own access(BYOA) hace que listar las aplicaciones permitidas sea extremadamente dificil. O que pasa si tenemos una aplicacion permitida a la que se le detecto una vulnerabilidad, dejando el camino libre a los atacantes, ya que este tipo de proteccion no puede hacer nada para proteger al endpoint.

## Anomaly-Based Detection

Esta aproximacion que usa algoritmos matematicos para detectar actividad inusual, se le llama como basados en heuristica, comportamiento o detector de anomalias. 

Estas se basa en establecer un comportamiento normal, y detecta todo lo que este fuera de este. Pero tiene un problema de que necesita grandes cantidades de datos para reducir los falsos positivos. 

## Anti-Spyware

Es muy similar a un antivirus tradicional, porque usa firmas para buscar los virus y el malware. 

## Firewalls

Los firewalls han sido una pidra angular de la seguridad de las redes desde los inicios de internet. Este es una plataforma de software o hardware que controla el flujo de tráfico en tre una red de confianza y una red no fiable. Aunque ambos protegen sus datos lo hacen de formas diferente. 

### Differences Between Personal Firewall and Network Firewalls

#### Personal Firewall

Estos suelen funcionar como firewalls de capa 7, que permiten o bloquean el trafico en fucnion de una politica de seguridad individual o de grupo. 
Son utiles en ordenadores portatiles utilizados por usuarios remotos que viajan y que conectar sus ordenadores a internet. Y puede controlar el trafico saliente, Sin embargo eludir estos firewalls es el pan de cada dia para los malwares mas complejos. 

#### Network Firewall

Estos protegen la red de una empresa contra amenazas procedentes de redes externas como internet. Sin embargo la mayoria de los que son basados en puertos hacen poco por proteger los endpoints dentro de la red contra amenazas que se originan dentro de la misma. 

## Host-Based Intrusion Prevention Systems

Se basan en un agente instalado en el endpoint para detectar el malware. Dado que un hips puede basarse en firmas o anomalias, es susceptible a sufrir los mismos problemas que otros enfoques basados en firmas y anomalias. Y aparte de degradar de gran manera el rendimiento de los endpoints. 


