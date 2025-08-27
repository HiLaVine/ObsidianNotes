# 1. Logs and Events

## Utilizing Logs and Telemetry for Incident Investigation

Dependiendo el sistema operativo de los endpoints, los equipos de seguridad usaran logs, que incluyen alertas y eventos mientras ellos investigan incidentes. 

Los logs de estos endpoints, ayudan a los equipos de seguridad a determinar la atribucion, spot de la actividad maliciosa e identificar victimas. Pero si la empresa no cuenta con host sofisticados o sistemas de gestion de redes, saber donde esta localizado un endpoint o usuario es dificil. 

Y para eso sirve recoletar los metadatos y la telemetria de los equipos. Siempre que se recolecte la informacion correcta y mas util. 

La informacion que normalmente se recolecta de los endpoints y que se analiza por los equipos de seguridad, son la ip, DNS hostname, application logs, procesos corriendo en la máquina. 

### Mejores practicas para la gestion de logs

* Rapid Turnover: Esto se refiere al cambio rapido de la informacion en los sistemas, debido a los protocolos de direccion dinamica y a los protocolos de asignacion dinamica. Ya que gracias a estos, un usuario puede tener una ip en un momento y luego tener otra en otro momento, o una ubicacion diferente.
* Log levels Based-On evironmental factors: Aquí se habla de que el nivel de los logs recopilados depende de los factores como el almacenamiento, el ancho de banda, y la capacidad de analizar estos logs.
* SIEM solution: Tener logs detallados es muy util en las investigacionse forenses para saber que paso despues de un ataque. Tipicamente en un SOC, los logs son enviados desde un endpoint a un SIEM, que los recolecta desde cualquier tipo de fuente, como firewalls, IDS e IPS, EDR y XDR, etc.
* Mobile Device Management: Los equipos moviles y las politicas de bring your own device (BYOD) crean su propios desafios. Los equipos moviles debido a sus caracteristicas y sus limitaciones naturales, como restrciciones del sistema y recursos del dispositivo. Muchas organizaciones usan plataformas de gestions de equipos moviles para manejar las politcas en estos mismos.
* Server logs: Es importante analizar los server logs. Las organizaciones analizan los mensajes simples de syslog, de servidores web, o archivos, regitros de aplicacion que se ejecutan en un servidor. No importa si es fisico o una VM, se debe aprovechar las capacidades de generar logs de estos. Como en un sistema unix, donde puedes ver los logs en /var/log.

## Windows Endpoint Logs and Events

Los analistas de seguridad pueden analizar e investigar varios tipos de logs, y son los siguientes: 

* Application logs: Contiene eventos de diferentes aplicaciones. 
* System logs: Incluye eventos de la operaciones de drivers, procesos y hardware.
* Setup logs: Contiene información sobre instalacion de software, como actualizaciones. 
* Security logs: Contiene eventos relacionados con seguridad, como intengos de logueo, operaciones relacionadas con archivos y objetos y gestion de accesos. 
* File logs: Contiene eventos de escritura o lectura de archivos y accesos.

### Tipos de eventos

* Error: Indica un problema importantecomo perdida de informacion o de funcionalidad. 
* Warning: Un evento no necesariamente importante, pero que puede ser un problema a futuro. 
* Information: Evento que describre el exito de una operacion, driver o servicio. 
* Success Audit: Evento que registra un intento de acceso exitoso. 
* Failure Audit: Un evento que registra un intento fallido de acceso a la red.

## Windows System Logs

Los mensajes de exito o fracaso alimentan los logs de seguridad. En windows los logs de seguridad los lleva el Local Security Authority Subsystem Service (LSASS) que corre con el nombre de lsass.exe y que se ejecuta en el directorio de System32. 

# 2. Endpoing Security Alerts

## Security Alerts and Alert Source

Las alertas de seguridad son generadas por diferentes herramientas, sistemas y equipos de seguridad. Estas toman diferentes formas dependiendo la fuente, como los syslog, que tienen una severidad que ayuda a los analistas de ciberseguridad a prestar mas atencion a esto. 

Las alertas tienen 6 tipos de información, espacios de tiempo, detalles  para identificar el sistema o equipo que genero la alerta. 

### Fuentes de informacion

Las alertas se pueden originar de varias fuentes. Los mas comunes son los NGFW y los firewall de host en los endpoints. Gestion de assets y monitoreo de sistemas. De HTTP, DNS, transacciones TCP, logs URL, y mensajes syslog de multiples fuentes. 

## Alert Evaluation and Classification

El panorama de las amenazas cambia y evoluciona constantemente con nuevas vulnerabilidades, y nuevas amenzas. Los atacantes saben esto y se aprovechan para cambiar y mejorar las caracteristicas de sus exploits y evadir la seguridad. 




