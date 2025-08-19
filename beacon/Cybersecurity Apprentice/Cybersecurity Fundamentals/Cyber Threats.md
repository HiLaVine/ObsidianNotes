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

## Ramsomware Types

El ransomware criptografico es el mas comun y exitoso de los tipos de ransomware que existen, pero no es el unico. Recordando que el ransomware no solo es una familia de malware, tambien es un modelo de negocio criminal que es usado para bloquear algo de valor por un rescate (Ransom). 

### Introduccion avanzada al Ransomware

Usar algo de valor para obtener dinero de un rescate no es algo nuevo, pero si muy lucrativo, y mas el ransomware. Ya que no tiene solo como objetivo los grandes negocios, si no tambien a personas individuales. Por lo tanto es facil generar una remuneracion y es mas rapido que otros cibercrimenes. Tambien es importante señalar que despues del pago es incierto si el atacante desencripte la informacion, y que seguramente esta ya haya sido vendida en la dark web por un poco mas dinero. 

### Ataques de ransomware en organizaciones

El malware desplegado en los ataques de ransomware criptografico no es precisamente sofisticado, pero ha sido provado que es realmente efectivo tanto en las ganacias del atacante, si no tambien en las consecuencias que deja en las organizaciones de continuar con sus operaicones normales. Y debido a que existen tantos objetivos potenciales, tanto chicos como grandes, ha promovido esto a tal punto que se lanzan nuevas campañas de ransomware todo el tiempo. 

### El ataque se hace en 5 etapas

Si el atacante falla en cualquiera de estos pasos, se considera que fue un fracaso, y para que un ataque sea exitoso, se deben seguir los siguientes 5 pasos: 

1. Compromise and Control a System or Device: este empieza normalmente usando ingenieria social para engañar a los usuarios, esto permite a los atacantes instalar malware en el sistema y tomar el control. 
2. Prevent Access to the System: Los atacantes deben idenrificar y encriptar cada archivo que parezca importante o denegar el acceso al equipo. 
3. Notify Victim: Atacante habla con la victima y establece los parametros del rescate.  
4. Accept Ransom Payment: El atacantes recive el pago evadiendo las leyes, usadon criptomonedas. 
5. Return Full Access: Los atacantes regresan el acceso a los dispositivos, y si no restauran, el plan pierde eficacia, debido a que la victima da todo por perdido y no paga.

## Vulnerabilities and Exploits

Los exploits y las vulnerabilidades puedes ser explotados para forzar a los softwares a actuar de formas para las que no fue planeado. Como recopilar información sobre las medidas de seguridad usadas actualmente. 

### Vulnerabilities

Estas son rutinariamente descubiertas en el software en un ritmo alarmante. Estas son mas comunes en software que acaba de ser terminado y desplegado, tambien pueden ser creadas inadvertidamente o reintroducidas cuando hay actualizaciones de seguridad. 

### Exploit

Un exploit es un tipo de malware que toma ventaja de una vulnerabilidad en un endpoint o servidor infectado. Estos son creados por el atacante con el objetivo de atacar a las vulnerabilidades caunsando que el software ejecute funciones o codigo en nombre del atacante. 

### Parchear vulnerabilidades

Los parches de seguridad son desarrollados por los software vendors lo mas rapido posible despues de que una vulnerabilidad sea descubierta en el software. 

1. Discovery: el atacante aprende sobre la vulnerabilidad y empienza el ataque antes de que el vendor descubra dicha vulnerabilidad o desarrolle un parche de seguridad.
2. Desarrollo del parche: el tiempo que tarda entre que se descubre una vulnerabilidad y se desarrolla y publica el parche se le conoce como amenaza Zero-day.
3. Test y despliegue del parche: Pueden pasar meses o años antes de que una vulnerabilidad sea anunciada al publico. Una vez que se dispone de un parche de seguridad, las organizaciones necesitan tiempo para probarlo adecuadamente e implementarlo en los sistemas afectados y durante este tiempo los sistemas que ejecutan el software son vulnerables.

### Como se ejecutan los exploits

Los exploits pueden estar incrustrados en archivos de datos aparentemente inofensivos, o pueden dirigirse a servicios de red vulnerables. Estos son peligrosos porque suelen estar empaquetados en archivos legitimos que no activan el software antimalware y por lo tanto no se detectan facilmente. 

1. Creación: La creación de un archivo de datos (exploit) es un proceso de dos pasos. El primer paso es incrustar un pequeño fragmento de código malicioso dentro del archivo de datos. Sin embargo, el atacante aun debe engañar a la aplicacion para que ejecute el codigo malicioso. Por lo tanto, la segunda parte, suele implicar técnicas de corrupción de memoria que permiten insertar codigo del atacante en el flujo de ejecucion del software.
2. Accion: Una vez creado el archivo de datos del exploit, una aplicacion legitima como un visor de documentos o un navegador web, realizara acciones en nombre del atacante, como establecer comunicacion y proporcionar la capacidad de cargar malware adicional en el punto final de destino. Dado que la aplicacion se explota es una aplicacion legitima, los antivirus tradicionales basados en firmas y el software de listas blancas no tienen practicamente ninguna defensa contra estos ataques.
3. Tecnicas: Aunque existen miles de exploits, todos ellos se basan en un pequeño conjunto de técnicas básicas. Algunos ataques pueden implicar mas pasos y otros menos, pero normalmente se deben utilizar entre tres y cinco tecnicas basicas para explotar una aplicacion. Independientemente del ataque o de su complejidad, para que el ataque tenga exito, el atacante debe ejecutar una serie de estas tecnicas basicas de explotacion en secuencia.
4. Heap Spray: Esta es una tecnica usada para facilitar la ejcucion de codigo arbitrariamente con la inyeccion a ciertas secuencias de bytes en la memoria o el proceso objetivo.

### Linea de tiempo para eliminar una vulnerabilidad

Las vulnerabilidades pueden ser explotadas desde que el software es desarrollado hasta que se parchea. 

1. Desarrollo de software
2. Descubrimiento de vulnerabilidades
3. Inicio de los exploits
4. Anuncio publico de las vulnerabilidades
5. Publicacion del parche
6. Desarrollo del parche
7.  Protegido por parche del proveedor

