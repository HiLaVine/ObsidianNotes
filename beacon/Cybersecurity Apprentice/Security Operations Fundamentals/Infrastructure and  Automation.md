# SOAR Technology

## SOAR Component

SOAR o Security Orchestration, Automation, and Response cuenta con tres componentes: 

* Orchestration: Este se encarga de activar y controlar el stack de los productos de seguridad desde una locacion central. Los productos SOAR hacen esto a traves de playbooks, que son flujos de trabajo basados en tareas que coordinan personas, procesos y tecnologias.
* Automation: El segundo componente de un SOAR es la automatizacion, el cual es el subset logico de la orquestracion. Con el SOAR, la automatizacion implica encontrar tareas repetibles y ejecutarlas a la velocidad de la maquina. Los productos SOAR cuentan con scripts de automatizacion e integraciones de productos extensibles para lograrlo.
*  Response: El componente final es la Respuesta, esto implica mantener la supervicion del incidente a lo largo de su ciclo de vida. En los productos SOAR, esto incluye la gestion de casos, la colaboracion durante la investigacion y el analisis y la elaboracion de informas tras el cierre del inicidente.

## The Importance of SOAR

SOAR está diseñado para la orquestacion automatizada de la interacción entre todos los elementos y para proporcionar la coordinacion de estas interacciones. SOAR es fundamental para el futuro de las operaciones de seguridad. 

Y tiene un valor añadido en que reduce el tiempo de respuesta y el riesgo, aumenta la eficiencia automatizando tareas y retiene el personal. 

## SOAR Systems

Los sistemas SOAR permiten acelerar la respuesta ante incidentes mediante la ejcucion de guias de actuacion entandarizadas y automatizadas de funcionan a partir de datos proceentes de tecnologias de seguridad y otros flujos de datos. Casí todas las organizaciones que se toman en serio la segruidad tienen un SIEM en su entorno. 

### SOAR 

Las herramientas SOAR recopilan alertas agregadas de fuesntes de detección (como el SIEM, herramientas de seguridad de red y buzones de correo) antes de ejecutar guías automatizables y basadas en procesos para enriquecer y responder a estas alertas. Las guías coordinan tecnologias, equipos de seguridad y usuarios externos para centralizar la visibilidad y accion de los datos. Ayudan a acelerar los tiempos de respuesta ante incidentes y aumentan la productividad de los analistas. Dado que las guías estandarizan los procesos, lo que genera una mayor coherencia, mejora la confianza en el funcionamiento de las capacidades de las operaciones de seguridad. 

### SIEM

Estos recopilan datos dispares y los agregan en las alertas. Las herramientas SIEM y las herramientas de orquestacion tienen algunas similitudes en la superficie como la automatizacion de acciones, la integracion de productos y la correlación de datos. Las herramientas SIEM supervisan fuentes de datos de máquinas, los correlacionan y agregan para contextualizarlos, y proporcionan detección y supervición en tiempo real de las alertas generadas por las aplicaciones y el hardware de la red. 

## Parts of Security Orchestration

La Security Orchestration es un metodo que conecta tecnologias de seguridad dispares, estandarizando y automatizando los flujos de trabajo lo que permite a los equipos de seguridad sacar adelante de forma eficiente la respuesta a incidentes y las operaciones de seguridad. Y tiene tres partes importantes: tecnologias de seguridad, playbooks/flujos de trabajo y equipos de seguridad. 

### Tecnologias de seguridad

Las herramientas SOAR se integran con otras herramientas ya sean de seguridad o no, para ayudar a los equipos con una consola centrol donde se coordinan y activan estas herramientas. Esta integracion activa las conversaciones entre productos, transferencia de datos y ejecucion remota de comandos.

Dicha integracion entre productos, puede ser unidireccional o bidireccional. La primera solo sirve para la transferencia de datos de una herramienta integrada a la herramienta de orquestacion. Y en la bidireccional se tiene una conversacion entre ambos productos. 

### Playbooks/Flujos de trabajo

Los playbooks son flujos de trabajo graficos basados en tareas que ayudan a vizualizar los procesos a lo largo de los productos de seguridad. Estos playbooks pueden ser automaticos, manuales o ambos. 

Y los playbook tienen los siguientes bloques:

* Playbook Trigger: Diseñado para ejecutarse automaticamente dentro de una herramienta de orchestration que necesita un punto de activacion. Este puede ser una condicion que una vez cumplida, se inicia el playbook. Por ejemplo un correo de phishing, que active el playbook de phishing. 
* Automated Playbook Task: Estas son tareas que se ejecutan de forma automatizada, ejecutando un codigo ya sea seleccionado o hecho por el cliente. 
* Manual Playbook Task: Son abstracciones en las que los usuarios pueden introducir cualquier comentario o instrucciones sobre cosas que se tienen que hacer de forma manual. 
* Conditional Task: Se pueden utilizar para comprobar el valor de cualquier artefacto relacionado con un incidente y ejecutar ramificaciones en funcion del resultado. Osea ejecutar diferentes tareas si una alerta es alta, media o baja.

#### Common SOAR Playbooks

Los playbooks mas usados son los siguientes: 

* Phishing Enrichment and Response: Este consume alertas de buzones de email, y coordina acciones con las herramientas como sandboxes, EDR, para tener una respuesta correcta.
* Threat Hunting: Estos pueden ser agendados para correr cada cierto tiempo, escanean buscando amenazas en el ambiente y consumen hilos de amenazas externas o realizar un seguimiento de incidentes existentes.
*  IoC Enrichment: estos pueden automatizar el enriquecimiento de los indicadores mediante la consulta de diferentes herramientas de inteligencia sobre amenazas para obtener contexto y presentar las resultados a los analistas, lo que ahorra tiempo y les da espacio para ser proactivos.
*  Incident Severity Assignment: Pueden asignar de forma automatica la severidad de los incidentes en base a sus parametros relevantes para la organizacion.
*  Cloud Security Orchestration: Coordinan la respuesta a traves de ambientes On-Premises y en la nube. Puede bloquear IoC maliciosos en los dispositivos de la nube y en el firewall local.

### Equipos de seguridad: 

Los playbooks SOAR, le permiten a los equipos a llevar la respuesta a incidentes y operaciones de seguridad de forma mas eficiente. 

Y los equipos se ven ayudados de la siguente manera: 

* Manual Task: Cuando una tarea es unica, matizada o infrecuente para ser automatizada, los playbook tienen tareas manuales que actuan como directivas para los especialistas de SecOps y que se ocupen del incidente.
* Task Approval: Incluso si algunas tareas pueden ser automatizadas, pueden existir taras muy sensibles, que necesitan la supervicion de una persona. Y esperan a la autorizacion de los especialistas de SecOps antes de ser ejecutadas.
* End-User Engagement: Una herramienta SOAR, que tiene inegraciones con herramientas de correo, puede ser usada por los analistas SecOps y usuarios finales en la organizacion para mejorar los procesos. 

## Security Gaps and Risks

Todos los retos de seguridad preocupan porque la mayoria representa un riesgo financiero o al negocio. Algunas brechas no crean riesgos financieros serios, pero otros son devastadores. Y hacen mucho daño a la reputacion de la empresa, especialmente si datos sensibles es publicado en linea. 

## How Security Orchestration Fills Gaps

Hay lagunas criticas que todavia existen en la seguridad. Esta sufre cuando se tiene mucha informacion pero poco seguimiento, falta de interconectividad, y una plantilla muy poco compartimentada. Y aqui las herramientas SOAR hacen su trabajo ya que aprovechan la ingesta y correlacion de datos de multiples fuentes, una red de integracion de productos extensible, manuales y funiones de colaboracion que democratizan las conocimientos del equipo. 

Y tiene los siguientes beneficios: 

* Accelerates Incident Response
* Standardizes and Scales Process
* Unifies Security Infraestructure
* Increases Analyst Productivity
* Leverage Existing Investments
* Improves Overall Security Posture

