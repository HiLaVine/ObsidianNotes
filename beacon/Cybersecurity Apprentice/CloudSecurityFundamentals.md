## 1. Virtualization, Containers and Micro-VMs

### Cloud Native Technology Properties

La Cloud Native Computing Foundation´s (CNCF) define las sigueitnes tres propiedades las cloud native technologies: 

* Container Packaged:  correr aplicaciones y procesos en un contendor de software como unidades aisladas del despliegue de la aplicación y como mecanismo para lograr un alto nivel de aislamiento de recursos. Esto mejora la experiencia general del desarrollador, fomenta el reusar codigo y simplifica las operaciones para las tecnologias nativas en la nube.
* Dynamically Managed: Programación y gestión activas mediante procesos centralizados. Mejora radicalmente la eficiencia de la máquina y la uilizacion de los recursos, al tiempo que reduce el coste asociado al mantenimiento y las operaciones.
* Microserviced: Acoplamiento flexible con dependencias descritas explicitamente. Aumenta sifnificativamente la agilidad general y la capacidad de mantenimiento de las aplicaciones.

### Important Terminology

* Hypervisor: Permite multiples sistemas operativos virtuales o invitados operar de forma concurrente en un solo host fisico.
* Native (Nativo): (tambien conocido como de Type 1 o bare metal) Un hypervisor nativo corre directamente en el hardware fisico del host (en el servidor)
* Hosted (Alojado): Un hypervisor hosteado corre en un entorno con un sistema operativo.

## Virtualization

La virtualización es la fundación del computo en la nube. Y la puedes ver como crear muchas maquinas virtuales para correr en un solo host fisico. 

### Hypervisor

Este es un software que permite correr de forma simultanea multiples sistemas operativos de forma virtual en un mismo host fisico. 

Existen dos tipos de hipervisores: 

* Type 1: Nativo, que como se menciono anteriormente es cuando se instala el software de hipervision directamente en el hardware del host fisico. Sin un sistema operativo instalado antes de el.
* Type 2: Hosteado, que se caracteriza por correr sobre un SO instalado dentro del host fisico.

### Security Considerations

La virutalizacion es una tecnologia muy importante usada en data centers y computo en la nube, usado para optimizar recursos. 

* Máquinas virutales durmientes: este es un problema común, ya que es común que muchas maquinas virtuales se encuentran dormidas y en desuso. Y el problema surge cuando se mantienen apagadas mucho tiempo, debido a que eso significa que se puede omitir la instalación de los sofwares de proteccion mas recientes y los parches de seguridad.
* Hypervisor vulnerabilities: esto aplica directamente al software del hypervisor, ya que puede tener problemas de seguridad.
* Intra-VM Communications: El trafico de red entre hosts virtuales, especialmente en un único servidor físico, puede no atravesar un switch físico. Esta falta de visibilidad aumenta la complejidad de la resolución de problemas y puede incrementar los riesgos de seguridad debido a las capacidades inadecuadas de supervición y registro.
* Expanción de las maquinas virtuales: los entornos virtuales pueden crecer con rapidez, lo que provoca un coalpso de los procesos de gestion de cambios y agrava los problemas de seguridad, como las MV inactivas, las vulnerabilidaes del hipervisor y las comunicaciones entre las MV.

## Containers

Un contenedor es un paquete de software que permite correr aplicaciones independientemente del sistema operativo del host.

### Container Orchestration

Kubernetes es una plataforma open source que provee una API(application programming interface) que ayuda a los desarrolladores a definir la infraestructura del contenedor como IaC (Infraestructure as Code).

Las organizaciones pueden aprovechar la orquestracion de kubernetes y una arquitectura de microservicios para publicar, mantener y actualizar aplicaciones nativas de la nube en contenedores de forma rapida y a escala. 

Los microservicios, son una arquitectura de desarrollo de software que usa contendores para dividir una aplicacion empresarial grande en pequeños conjuntos para que los programadores trabajen en ellos. Estos microservicios corren en contendores separados y kubernetes orquesta estos contenedores para ejecutar todo el código de la aplicaicion. 

### Containers as a Service

Mientras los contenedores crecian en popularidad y se diversificaban, los orquestadores como kubernetes y sus derivados como OpenShift, mensos y Docker Swarm tomaron una gran importancia en el desarrollo, operación y escala de los contenedores. Y ahí las plataformas Containers as a Service (CaaS) son tan importantes debido a que se encargan de administrar todo el funcionamiento de estos. 

Estos abstraen mucho la complejidad requerida para el despliegue y operacion de un gran conjunto de microservicios, estos son mas complejos de configurar y mantener. Estos orquestadores se centran en el tiempo de ejecución del contenedor y hacen poco para ayudar con el despliegue y la gestión de los hosts subyacentes. 

Aunque las organizaciones sofisticadas suelen utilizar tecnologías como las máquinas virtuales ligeras envueltas en herramientas de automatización para solucionar este problema, ni siquiera estos enfoques liberan por completo a la organización de la gestión del hardware de computación, almacenamiento y red subyacente.

## Hypervisor VS Docker Containers

Existen muchas diferencias entre los contendores y el hipervisor, pero la principal es que un hipervisor abstrae hardware y te permite correr sistemas operativos completos. Y y los contendores abstraen el sistema operativo para correr aplicaciones. 

## Micro-VMs






