# 1. Application Development Platforms and Processes

## Cloud Native Security Platform (CNSP)

El acercamiento del cloud native toma lo mejor que puede ofrecer la nube, como la escalabilidad, capacidad de implementación, facilidad de gestión, y potencia informática ilimitada bajo demanda y aplica estos principios al desarrollo de software, en combinación con la automaizacion de CI/CD, para aumentar radicalmente la productividad, la agilidad empresarial y el ahorro de costes. 

### CI/CD (Continuos Integration/Continuos Delivery)

Las metodologias para el desarrollo de aplicaiones estan evolucionando lejos del tradicional cascada, a modelos mas agiles. 

Los beneficios y retos del CI/CD son los siguientes: 

* Beneficios: CI/CD es un nuevo acercamiento que ofrece muchos beneficios, como un tiempo de comercializacion mas corto y una entrega de software mas eficiente.

* Retos: Las metodologias tradicionales de seguridad, no fueron diseñadas para los flujo de trabajo modernos. Ya que los equipos de desarrollo adoptan tecnologias nuevas basadas en la nube y los equipos de seguridad se quedan atras. Lo que hace que surga un nuevo enfoque de seguridad completamente nuevo, ya que los factores de riesgo aumentan el riesgo de compromiso y probabilidad de que se produzcan violaciones de seguridad.

### Arquitecturas nativas en la nube. 

Estas consisten en servicios en la nube como contenedores, seguridad serverless, PaaS (Platform as a Service) y microservicios. 

Estos servicios estan ligeramente aclopados, lo que significa que no estan conectados de forma fija a ningun componente de la infraestructura, lo que permite a los desarrolladores realizar cambios con frecuecia sin afectar otras partes de la aplicacion ni a los proyectos de otros miembros del equipo. Esta fue desarrollada de forma nativa para la nube. 

### DevOps, SecOps, and DevSecOps

Nacidadas debido que la complejidad, costo y riesgo se fueron incrementando con el uso de mas herramientas y fabricantes diferentes implementados como medidad de seguridad, se necesitaba una forma de integrar todo en una sola plataforma que fuera compatible con el ciclo de vida de CI/CD y el flujo de trabajo de DevOps. 

* DevOps: es la colaboracion entre el team de desarrollo y el de IT, teniendo una realción mas cercana con todos los equipos facilitando el lanzamiento de las aplicaciones. 
* SecOps: Este es esecialmente el team de IT pero enfocado en la seguridad. Ya que en el pasdo el IT team y el team de seguridad eran dos diferentes, pero ahora son el mismo haciendo todo mas seguro desde su inicio. 
* DevSecOps: Este tiene un enfoque mas en la asegurar la seguridad que el DevOps y SecOps. Ellos se centran en aplicar y automatizar procesos mas seguros a lo largo del proceso de CI/CD.

### Funciones del CNSP

Tiene 3 funciones que son: 

* Visibilidad: Provee una visibilidad unificada para los equipos de SecOps y DevOps.
* Integracion: Proporciona un conjunto integrado de capacidades para responder a las amenazas y proteger las aplicaciones nativas en la nube. 
* Automatizacion: Que las correcciones de vulnerabilidades y configuraicones incorrectas sean de forma automatica, siempre de forma coherente en todo el ciclo de vida.

## Security and Cloud Application Development

El desarrollo en la nube debe sguir el proceso del CI/CD, y en optimas situaciones las operaciones de seguridad se integran en este flujo. El proceso CI/CD, tambien llamado proceso DevOps, es el flujo de trabajo en el que se intregan los procesos que intervienen en el flujo de trabajo de la entrega de software. 

## DevOps Software Development Model

Este modelo esta remplazando al tradicional ciclo de vida. 

### Caracteristicas importantes 

DevOps unifica los teams de desarrollo y operaciones a lo largo del proceso de entrega de software, ayudando a la pronta deteccion y arreglo de problemas, automaizando el testing y desarrollo y reduce el tiempo de comercializacion. 

Y las caracteristicas importantes son: 

* Equipos colaborativos: Los equipos de desarrollo y operaciones trabajan en comunicacion y colaboracion. 
* Cultura: se refiere a una cultura de coperacion en todo el ciclo de entrega. 
* Estrategia: se tiene herramientas que trabajan en conjunto con el modelo DevOps, ya que este es una estrategia no una herramienta. 
* Mas que automaizacion: es una clave del proceso de DevOps.

## Prioritizing Software Security in the Cloud

El cliente es el ultimo responsable por la seguridad de los datos, host contenedores y las instancias serverless en la nube. Ya que el public cloud service provider hace un gran trabajo con la construccion, mantenimienod y actualizacion del hardware, VM, data storage, y databases con el minimo de mecanismos de seguridad. 

## DevOps CI/CD Pipeline

DevOps es un ciclo CI/CD, osea un proceso CI/CD. 

## DevSecOps Software Development Model

Un problema en DevOps es que la seguridad queda en segundo plano, por lo que esta se mueve al desarrollo del codigo antes de su implementación. Y para arreglar esto, devido a lo comun que es avanzar en el desarrollo sin un chequeo de seguridad, se usa el DevSecOps. 

# 2. Security Operations Responsibilities

## What is Identity and Access Management (IAM) Security?

Es un parametro de seguridad en la nube que funciona para como una herramienta para mejorar la seguridad en la nube. Es parte de la seguridad en la nube. Cloud Infrastructure Entitlement Management (CIEM) se centra en detectar las diferencias entre los privilegios necesarios y los privilegios innecesarios. También proporciona visibilidad sobre los derechos que podrían suponer riesgos para la seguridad y aplica medidas correctivas para lograr un acceso con los mínimos privilegios.

## Alerts

Las alertas son una parte importante de la supervisión continua de todos sus entornos en la nube para detectar configuraciones incorrectas (como instancias de almacenamiento en la nube expuestas), amenazas avanzadas de red (como el criptojacking y la exfiltración de datos), cuentas potencialmente comprometidas (como claves de acceso robadas) y hosts vulnerables. Prisma Cloud correlaciona los datos de configuración con el comportamiento de los usuarios y el tráfico de red para proporcionar contexto sobre las configuraciones incorrectas y las amenazas en forma de alertas procesables.

### Notificaciones e integraciones

Además, Prisma Cloud ofrece la posibilidad de configurar integraciones externas en Prisma Cloud con tecnologías de terceros, como plataformas SIEM, sistemas de tickets, sistemas de mensajería y marcos de automatización, para que pueda seguir utilizando sus herramientas operativas, de escalado y de notificación existentes.

