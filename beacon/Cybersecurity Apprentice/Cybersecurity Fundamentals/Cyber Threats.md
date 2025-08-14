# 1. Malware types and Advanced Malware

## Malware and Ransomware

Malware (abreviación de "Malicious Software") es un archivo o código que típicamente quiere obtener el control, obtener información o dañarla de un endpoint infectado. 

### Definición y objetivos

El malware normalmente tiene alguno de los siguientes objetivos: 

* Control remoto de una máquina infectada.
* Mandar spam de una máquina infectada a otros objetivos. 
* Investigar la red local del usuario infectado. 
* Robar información sensible. 

Advanced/Modern Malware generalmente es como se le llama a malware nuevo o desconocido. Estos tipos de malware son altamente sofisticados y tienen objetivos específicos, además de eliminar de forma sencilla las defensas tradicionales. 

## Malware types

Este tiene una gran variedad de tipos y capacidades, y algunos ejemplos son los siguientes: 

* **Logic Bombs**: Es un malware que se dispara bajo una condición especial como una fecha o la desactivación de una cuenta de usuario concreta. 
* **Spyware y Adware**: Estos se caracterizan por que se centran en la recoleccion de informacion como el comportamiento de navegacion en internet, credenciales o informacion financiera. Por un lado el Spyware cambia configuraciones de los navegadores y otros softwares haciendo mas lenta la pc o el internet. Y el Adware es un tipo de spyware que desplega ads de forma molesta, incluyendo pop-up banners. 
* **Rootkits**: Este es un malware que da privilegios a nivel root de una computadora. Estos se instalan en la BIOS de la máquina lo que representa un problema ya que las herramientas de seguridad a nivel SO no las detectan. 
* **Bootkits**: malware conocido por ser kernel-mode, comunmente usado para atacar computadoras que tiene una proteccion de full-disk encryption.  
* **Backdoors**: Este tipo de malware le permite al atacante obtener acceso de una máquina comprometida sin tener que autenticarse. 
* **Anti-AV**: Esta es un tipo de malware que deshabilita software de antivirus legitimo en el equipo comprometido, así impidiendo la deteccion y eliminacion de otros programas maliciosos. 
* **Ramsomware**: Tipo de malware que bloquea  una computadora o equipo (locker ransomware) o que encripta información (Crypto ransomware) en un equipo infectado. Tendiendo solo acceso el atacante, por el cual se pide un rescate. 
* **Trojan Horses**: Este se distingue por dar al atacante el control completo de la máquina, incluyendo privilegios elevados. Y estos no se auto replican a diferencia de otros malwares. 
* **Virus**: Este es un tipo de malware que se puede auto-replicar, pero primero tiene que infectar un host y tiene que ser ejecutado por el usuario o un proceso. 
* **Worm**: Estos tipicamente atacan a una Pc o red y se pueden replicar rapidamente, pero a diferencia de otros tipos de malware este no es necesario que sea ejecutado por un usuario o proceso lo que lo vuelve muy peligroso. 

## Advanced or Modern Malware

Este es sigiloso y evasivo, aparte de jugar un rol importante en el ataque de un objetivo. 

Este malware aprovecha las redes para ganar potencia y resistencia. Aparte de que se puede actualizar como cualquier otra aplicación de software, de modo que un atacante puede cambiar de rumbo y profundizar en la red, o realizar cambios y aplicar contramedidas. 

Y esto es un cambio fundamental contra los tipos de malware anteriores, que solían ser agentes independientes que simplemente infectaban y se replicaban. 

### Tipos de malware avanzado

* **Obfuscation:** tipo de malware que usa técnicas de ofuscación para ocultar cadenas binarias que se usan en el malware y pasar inadvertidas. Esto ha evolucionado hasta poder ocultar un programa completo. 
* **Polymorphism:** Esto se logra cuando un programa malicioso contiene código enfocado en cambiar la firma del mismo programa, lo que produce un numero infinito de hash de firmas únicas. Con solo modificar un bit el hash cambia totalmente. 
* **Distributed:** Este aprovecha al máximo la resiliencia inherente a internet, teniendo múltiples servidores de control distribuidos por todo el mundo, o usando dispositivos zombie (infectado previamente) como canales de comunicación, lo que proporciona un numero casi infinito de vías de comunicación para adaptarse y actualizar el código según sea necesario. 
* **Multi-functional:** Actualizaciones de los servidores C2 también pueden cambiar por completo la funcionalidad del malware avanzado. Esto les permite atacar de forma estratégica para realizar tareas especificas, como el robo de números de tarjetas, envió de spam infectado o instalar ramsomware. 

# 2. Ransomware, Vulnerabilities, and Exploits

