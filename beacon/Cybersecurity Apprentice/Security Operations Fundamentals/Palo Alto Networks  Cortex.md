# 1. The Cortex Platform

## ¿Qué es Cortex?

Es una plataforma de seguridad continua basada en inteligencia artificial. Y que permite a las organizaciones crear, ofrecer y utilizar nuevos productos de seguridad innovadores de cualquier proveedor sin complejidad ni infraestructura adicionales. 

### Desired Security Features

* Prevent Data Breaches
* Prevent Cyberattacks
* Detect and Prevent Threats
* Simplify Investigations
* Simplify Management

Palo Alto Networks tiene diferentes acercamientos para los equipos de SecOps:

1. Previene todas las amenazas que pueda con la protección para endpoints Cortex XDR y nuestros firewalls de ultima generación. Todo lo que no pueda prevenir deberá detectarse e investigarse rápidadmente. Esto se consigue con Cortex XDR, Cortex XSOAR TIM, and Cortex Data Lake.
2. Se automatizan continuamente las respuestas con Cortex XSOAR. Y permite a los equipos de seguridad recopilar alertas de multiples fuentes y, ejecutar guias automatizables para acelerar la respuesta a incidentes.
3. Por último, se habilita la respuesta automatica en el tiempo real ane amenazas con Cortex XSIAM. Esta es una plataforma de operaciones se seguridad basada en IA que revoluciona la forma en que se implementan los datos, los análisis y la automatización para adelantarse a las amenazas modernas.
4. Cortex es la plataforma para SecOps, se aceleran investigaciones al disponer de los datos adecuados, integrados en la red, endpoints y la nube.

# 2. Cortex XDR

## Stop Malware and Ransomware

El agente de Cortex XDR previene la ejecucion de archivos maliciosos con un acercamiento personalizado para combatir tanto ataques tradicionales como modernos. Adicionalmente, los administradores pueden usar periodicamente escaneos para identificar amenazas latentes, cumplir con los requisitos normativos y acelerar la respuesta antes incidentes con el contexto de los endpoints. 

El cortex tambien puede hacer calendarizar o hacer escaneos sobre demanda para detectar malware en archivos de office con macros, archivos ejecutables, y librerias de enlace dinamicas (DLLs) para mitigar estos sin abrir los archivos maliciosos. Con Cortex XDR, se puede mitigar con malware conocido y desconocido incluyendo ransomware. 

## Behavioral Threat Protection

Los ataques mas sofisticados usan multiples apliaciones y procesos legitimos para sus operaciones maliciosas, y se han vuelto muy comunes, lo que hace sean dificiles de detectar y requerir una visibilidad mas profunda para correlacionar este comportamiento malicioso. Para que la proteccion basada en comportamiento sea efectiva, incluyento la identifiacion de la actividad maliciosa ocurriendo con procesos legitimos, es critico entender todo lo que pasa en el endpoint. El agente cortex XDR usa la proteccion basada en comportamiento en diferentes maneras. 

El ciclo de vida de la protección contra amenzas de comportamiento son: 

1. Endpoint Attacks Generate Multiple Events
2. Cortex XDR Executes Policy-Based Action
3. Cortex XDR Prevents Script-Based, File-Less Attacks
4. Cortex XDR Blocks Ransomeware

Cortex XDR Prevent ==> Silent behavioral rules for prevention ==> Active behavioral rules for prevention ==> Behavioral rules for detection and response

## Technique-Based Exploit Prevention

El agente Cortex XDR previente vulnerabilidades conocidas, zero-day y no parcheadas, mediante el bloqueo de tecnicas de exploits que los atacantes usan para manipular aplicaciones. Y existen muchos exploits, por lo general, se basan en un pequeño conjunto de técnicas de explotación que cambia con poca frecuencia. Cortex XDR evita los intentos de explotación antes de que los endpoints puedan verse comprometidos. 

Cuando es necesario realizar una reparación en el punto final tras una alerta o una investigación, los administradores tienen la opción de tomar las siguientes medidas:

* Isolate Endpoints
* Terminate Processes
* Block Additional Executions
* Quarantine Malicious Files
* Retrieve Files
* Access Endpoints with Live Terminal
* Orchestrate Response

# 3. Cortex XSOAR

## Palo Alto Network SOAR Solution

El Cortex XSOAR combate los retos de seguridad con tres areas principales: Workflow automation, ticketing and collaboration. 

Alert sources ==> Respond and Automate ==> Manage Incidents ==> Collaborate and Learn

* Respond and Automate: La primera area de trabajo en el Cortex XSOAR es la automatizacion del flujo de trabajo, con una integracion de la red con todos los productos ya sea de seguridad o no. Todo basado en el playbook que se haya definido.
* Ticketing: La segunda area es la gestion y ticketing. El XSOAR puede obtener toda la informacion de las fuentes de informacion como SIEMs, herramientas de seguridad de redes, buzones de email, manejo de vulnerabilidades y soluciones de seguridad en la nube. Se puede colocar un SLA con un playbook, para manejar de forma correcta y estandarizar procesos a lo largo de los equipos, productos, y casos de uso. Y siempre adaptandose a las amenazas emergentes.
* Collaborate and Learn: La tercera area es la colaboracion e investigacion en tiempo real.

## Framework for SOAR Use Cases

* Security Operations: Ejemplos de este caso de uso con los password reset, unusual user travel, SSL certificate checks, and IT offboarding and onboarding.
* Cloud Security: Escanear es usado para coordinar las respuestas a lo largo de las infraestructuras tanto en la nube como on-premise.
* Vulnerability Management: El XSOAR puede obtener vulnerabilidades de Qualys y otros scanners. Los playbooks pueden automatizar el enriquecimiento de CVE y recolectar comentarios y diagnosticos de clientes.
* Los playbooks pueden coordinar la respuesta en la OT y IT. 

## The Goals for SOAR

El XSOAR provee a los SecOps de estas capacidades: 

* Accelerated Responses
* Standardized Process
* Collaboration and Learning
* Reduced Risk

# 4. Threat Intelligence Management

La inteligencia sobre amenazas es el núcleo de todas las operaciones de seguridad. Se aplica a todos los casos de uso de seguridad. Desafortunadamente, los equipos de seguridad están demasiado sobrecargados para aprovechar realmente su inteligencia sobre amenazas, con miles de alertas y millones de indicadores que reciben a diario. Necesitan contexto adicional, colaboración y automatización para extraer su verdadero valor. Necesitan una solución que les dé la confianza necesaria para hacer su trabajo de forma eficaz y reforzar sus defensas contra el próximo movimiento del atacante.

Cortex XSOAR TIM adopta un enfoque único para la gestión nativa de la inteligencia sobre amenazas, unificando la agregación, la puntuación y el intercambio de inteligencia sobre amenazas con la automatización basada en guías de procedimientos.

Las principales características y capacidades de Cortex XSOAR TIM incluyen:

* Powerful, native centralized threat intel
* Indicator relationships
* Hands-free automated playbooks with extensible integrations
* Granular indicator scoring and management
* Automated, multisource feed aggregation
* Most comprehensive marketplace

# 5. Cortex XSIAM
