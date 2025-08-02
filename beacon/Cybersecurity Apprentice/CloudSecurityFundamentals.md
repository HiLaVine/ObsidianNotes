# 1. Virtualization, Containers and Micro-VMs

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

Estas micro maquinas virtuales son extremadamente ligeras, ya que solo coneitneen el kernel de linux y las caracteristicas necesarias para correr en un contenedor. 

# 2. Serverless Computing and Function as a Service

Las arquitecturas serverless, tambien referidas como Function as a Service (FaaS), permite a las organizaciones construir y desplegar software y servicios sin mantener y provisionar un servirdor fisico o virtual. Las aplicaciones hechas con esta arquitectura son adecuadas para un gran rando de servicios y se pueden escalar mientras las tareas de la nube crecen. 

### Beneficios de usar computo serverless y FaaS

* Se centra en la funcionalidad basica del producto: Al no tener que usar parte de los recursos en tener la infraestructura y solo usar la nube, todo el trabajo se centra en el producto y sus caracteristicas. 
* No hay responsabildad por los parches de seguridad: El proveedor del servicio en la nube es el encargado de llevar a cabo todas las tareas de mantenimiento y seguirdad.
* Data Center seguro, redes y servidores: En esta arquitectura el proveedor es el responsable de la seguridad del data center, redes, servidores, SO, y sus configuraciones. 

### Adoptar el modelo serverless

* Reduccion de los gastos operativos
* Aumento de la agilidad y productividad
* Reduccion de costos

## Paquetes de aplicacion y ambiente del serverless

Aunque los contenedores bajo demanda reducen considerablemente la superficie expuesta a los usuarios finales y, por lo tanto, la complejidad asociada a su gestion, algunos usuarios prefieren una forma aún mas sencilla de impolementar sus aplicaciones. Serverless es una clase de tecnologias diseñadas para permitir a los desarrolladores proporcionar solo el código de su aplicación a un servicio, que luego instancia automaticamente el resto de la pila que hay debajo. 

* App Package: En aplicaciones serverless, el desarrollador solo carga el app package, sin ningun contenedor o componentes del sistemas operativos. La plataforma tomas los paquetes y los transforma en una imagen, y la corre en un contendor. En esta arquitectura los usuarios realizan las conseciones en cuanto a compatibilidad y control a cambio de la experiencia de implementación y gestion mas sencilla y eficiente.

* Ambiente serverless: Este incluye a los proveedores como amazon, azure, etc.

### Problemas con la arquitectura serverless

Esta arquitectura incluye nuevos problemas que tienen que ser considerados.

* Incremento de la superficie de ataque
* Mayor complejidad en la superficie de ataque.
* Un complejidad mayor en el sistema.
* Testeings indadecuados de seguridad.
* No se tiene la capacidad de usar protecciones de seguridad tradicionales.

### Herramientas comunes de escaneo.

* Dynamic Application Security Testing (DAST)
* Static Application Security Testing (SAST)
* Interactive Application Security Testing (IAST)







