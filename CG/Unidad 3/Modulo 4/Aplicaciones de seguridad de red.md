## FireWall

La mayoria de firewalls son similares en sus funciones basicas. Todos permiten trafico o lo bloquean en funicones de un congunto de reglas. Cuando los paquetes de datos entran en una red, el firewall inspecciona el encabezado del paqute para permitir o denegar su acceso en funcion de su nuermo de puerot.

**Los NGFW tambien puden inspeccionar cargusa utilies de paquetes y cada sistema debe tener su firewall independiente de de la red**

## Sistema de detección de intrucciones (IDS - Intruder Detection System) 

Es una aplicación que monitorea la actividad del sistema y alerta sobre psoibles intrusiones. Este alerta en función de la firma del trafico malicioso. 

El IDS está configurado para detectar ataques conocidos. Este suele detectar paquetes de datos a medida qu ese mueven por la red, y los analiza en busca de las caracteristicas de ataques conocidos. Alungos IDS revisan no solo las firmas de ataques conocidos, sino tambien las anomalias que podrian ser el signo de actividad maliciosa. Cuando el IDS detecta algo, envia una alerta al administrador lo mas pronto posible. 

## Sistema de prevención de intrusiones. 

El IPS es una aplicacion que monitorea la actividad del sistema en busca de actividad intrusiva y toma medidas para detenerla. Este a diferencia del IDS no solo notifica, si no que tambien detiene activamente las anomalias cuando se detectan. 

Un IPS busca firmas de ataques conocidos y anomalias de datos y bloquea un remitente especifico. Este al igual que el IDS se encuentra ya en la red segura despues del Firewall. Lo que mejora la seguridad ya que bloquea los flujos de datos peligrosos incluso si lograron pasar el firewall. 

Al ser un dispositivo inline, y necesita que el flujo de datos pase a través de el, si falla la conexion entre el internet y la red privada deja de funcionar. Y otro fallo es que se generan falsos positivos constantemente. 

## Dispositivos de captura de paquetes completos

Estos pueden ser muy utiles para administradores de red y profesionales de seguridad. Y permiten registrar y analizar todos los datos que se transmitesn a traves de la red. Ayuda a la investigacion de una alerta del IDS. 








