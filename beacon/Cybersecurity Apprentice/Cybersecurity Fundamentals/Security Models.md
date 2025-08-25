# 1. Security Models and Perimeter-Based Security

## Perimeter-Based Security Model

Los modelos de seguridad de red basados en el perimetro se remontan a los inicios de la era de los mainframes (a finales de la década de 1950), cuando los grades ordenadores mainframe se encontraban en salas de máquinas físicamente seguras. A estas salas solo podian acceder un número limitado de terminales de entrada remota conectados directamente al mainframe en areas fisicamente seguras. 

### Se basa en la seguridad física

A dia de hoy, los centro de datos actuales son el equivalente moderno de las salas de máquinas, pero la segruidad física basada en el perímetro ya no es suficiente. 

* Mainframe Computers: son anteriores al internet, de hecho, las computadoras mainframe son anteriores a ARPANET, que a su vez es anterior al internet. Hoy en día, un atacante utiliza internet para obtener acceso remoto, en lugar de violar físicamente el perímetro del centro de datos.
* Processing Power: El principal valor del ordenador centrl era su potencia de procesamiento. Los datos relativamente limitados que se producian se almacenaban normalmente en soportes near-line, como cintas. Hoy en día, los datos son el objetivo. Estos se almecenan en linea, en centros de datos y en la nube, y son un objetivo de gran valor para cualquier parte.
* Data Center: Hoy en día, millones de dispositivos periféricos remotos acceden a los centros de datos desde cualquier lugar, y en cualquier momento. A diferencia de los RJE de la era de los mainframes, lso dispositivos periféricos mdoernos, son mucho mas potentes que muchos de los primeros ordenadores mainframe y son ellos mismos objetivos.

### Assumes Trust on Internal Network

El principal problema de una estrategia de seguridad basada en el perimetro, que implementa contramedidas en unos pocos puntos de entrada y salida bien definidos de la red, es que dicha estrategia se basa en la suposicion dq ue todo lo que hay en la red interna es fiable. 

#### Distincion entre interno y externo

Los empleados remotos, usuarios moviles y las soluciones de computacion en la nube difuminan la disticion entre interno y externo. 

### Allows Unwanted Traffic

Un modelo de confianza roto no es el unico problema de los enfoques de seguridad de red centrado en el perimetro. Otro factor que contribuye es que los dispositivos y tecnologias de seguridad tradicionales (como los firewalls basados en puertos) que se utilizan habitualmente para construir perimetros de red dejan pasar demasiado trafico no deseado. 

Las deficiencias y limitaciones típicas de los enfoques centrados en el perímetro:

* Application Control: No puedo diferenciar de las buenas aplicaciones de las malas.
* Encrypted Traffic: No tiene en cuenta adecuadamente el trafico de aplicaciones cifradas.
* Identify Users: No controlo e identifica correctamente a los usuarios.
* Protect Against Attackers: No filtra el trafico permitido para amenazas conocidas transmitidas por aplicaciones o amenazas desconocidas.
* Net Result: Reestructurar las defensas para crear limites de confianza internos generalizados no es suficiente por si solo. Las organizaciones tambien deben asegurarse de que los dispositivos y tecnologias utilizadas para implementar estos proporcionen la visibilidad, control y capacidades de inspeccion de amenazas necesarias para habilitar de forma segura las aplicaciones empresarias esenciales y frutrar cualqueir ataque moderno. 

# 2. Zero Trust Security Model and Implementation

## Zero Trust Security Model

El modelo de seguridad Zero Trust aborda algunas de las limitaciones de las estrategias de seguridad de red basadas en el perimetro al eliminar la suposicion de confianza de la ecuacion. 

Con este modelo, las capacidades de seguridad esenciales de implementan de manera que se garantice el cumplimiento de las politicas y la proteccion de todos los usuarios, dispositivos, aplicaciones y recursos de datos, asi como el trafico de comunicaciones entre ellos, independientemente de su ubicacion. 

* No Default Trust: Con Zero Trust no existe una confianza predeterminada para ninguna entidad, incluidos los usuarios, dispositivos, aplicaciones y paquetes independientemente de lo que sea y de su ubicacion en la red empresarial o en relacion con ella.
* Monitor and Inspect: La necesidad de verificar siempre requiere una supervision e inspeccion continuas del trafico de comunidades asociado en busca de actividades subversivs.
* Compartmentalize: Los modelos Zero Trust establecen limites de confianza que compartimentan eficazmente los distintos segmentos del entrono informatico interno. La idea general es acercar la funcionalidad de seguridad a los recursos que requieren proteccion. De esta forma la seguridad siempre se puede aplicar independientemente del punto de origen del trafico de comunicaion asociado.

### Beneficios del modelo Zero Trust

En el modelo Zero Trust, verficar que las entidades autorizadas esten haciendo siempre solo lo que tienen permitido hacer no es opcional, es obligatorio. 

Y algunos beneficios son: 

* Improved Effectiveness: Mejora clara en la eficacia en la mitigacion de la perdida de datos gracias a la visibilidad y habilitacion de las aplicaciones, ademas de la deteccion y precencion de ciber amenazas.
* Greates Efficiency: Mayor eficiencia para lograr y mantener el cumplimiento de los requisitos de seguridad y privacidad mediante el uso de límites de confianza para segmentar aplicaciones, sistemas y datos confidenciales.
* Improved Ability: Mejora la capacidad para implementar de forma segura iniciativas de TI transformadoras, como la movilidad de los usuarios, politicas, virtualizacion y computo en la nube.
* Lower Total Cost of Ownership: Reduccion del coste total de propiedad con una plataforma operativa de seguridad con solidada y totalmente integrada, en lugar de una serie de productos de seguridad aislados y  diseñados para fines especificos.

## Zero Trust Design Principles

El principio del privilegio minimo en la seguridad de las redes se refiere a que solo se le dara el acceso minimo necesario para poder llevar a cabo sus labores sin problemas. 

### Principios del Zero Trust

Los perfiles de seguridad estan definidos en base a una auditoria de seguridad inicial llevada a cabo acorde a las politicas de inspeccion Zero Trust. De esta forma descubriendo que privilegios son esencales para que un dispositivo o usuario llevan a cabo sus funciones especificas. 

* Ensure Resource Access: Este principio sugiere la necesidad de establecer multiples limites de confianza y aumentar el uso de accesos seguros para la comunicación hacia o desde los recurso. Basicamente asegurarse de que se acceda a todos los recursos de forma segura, sin importar su ubicacion.
* Enforce Access Control: Adoptar la estrategia del minimo privilegio y reforzar el control de accesos minimizando dicho acceso  para reducir caminos dispobibles para que tanto el malware como el atacante gane acceso no autorizado.
* Inspect and Los All Trafic: Este principio reitera la necesidad de siempre verificar al tiempo que refuerza la idea de que una proteccion adecuada requiere algo mas que una aplicacion estricta del control de acceso.  

## Arquitectura Zero Trust

El modelo Zero Trust identifica la superficie protegida, que esta hecha por los mas valiosos y criticos datos, assets, aplicaiones y servicios. La superficie protegida de cada organizacion en unica, ya que solo contiene lo mas critico de la empresa, la superficie protegida es mucho mas pequeña que la superficie de ataque y siempre se puede conocer. 

### Identificar el trafico

Con el entnedimiento de las interdependencias que existen entre las organizaciones, infraestrcutura, servicios, y usuarios. El equipo de seguridad debe poner controles en los lugares mas cercanos a la superficie protegida posible. Creando así un micro perimetro alrededor que acompañe a donde sea a la superficie protegida. 

### Zero Trust Segmentation Platform

La segmentacion en la plataforma Zero Trust es el componente utilizado para definir los limites de confianza internos, y proporciona la mayor parte de las funciones de seguridad para cumplir con los objetivos operativos del Zero Trust. 

* Secure: Activa el acceso seguro a la red.
* Control: Controla de forma granular el flujo de tráfico hacia y desde los recursos.
* Monitor: Monitorea continuamente las sesiones permitidas por actividad sospechosa.

### Arquitectura conceptual

Con la superficie protegida identificada, los equipos de seguridad son capaces de identificar como el trafico se mueve a lo largo de la organizacion en realcion con esta misma. Entendiendo quienes son los usuarios, que aplicaciones usan, y como se conectan ya que esta es la unica forma de determinar y mejorar las politicas mejorando la seguridad de los datos. 

#### Fundamental Assertions about Zero Trust

* Siempre se asume que la red es hostil. 
* Las amenazas internas y externas siempre existen en la red todo el tiempo.
* La localidad de la red, nunca es suficiente para decidir la confianza en una red.
* Todos los dispositivos, usuarios y flujos de red se autentican y autorizan.
* Las politicas deben ser dinamicas y calcularse a partir del mayor numero posible de fuentes de datos.

## Zero Trust Conceptual Architecture

Los modelos de seguridad tradicionales identifican las areas en las que pueden producrise infracciones y exploits, la superficie de ataque y se intenta progeter toda la superficie. Desgraciadamente identificar toda la superficie de ataque es dificil debido a los multiples factores que la conforma. 

Por esto en el modelo Zero Trust, solo se concede accceso a la superficie protegida al trafico conocido y permitido. Una puerta de enlace de segmentacion, normalmente un NGFW es el que controla este acceso. Las politicas Zero Trust proporcionan un control granular, asegurando que los usuarios tengan acceso a los datos y aplicaiones que necesitan para realizar sus tarea y nada mas, cumpliendo el principio del minimo provilegio. 

### Zero Trust Least Privilege Access Mode

Para implementar el modelo de minimo privilegio en la red el firewall debe: 

* Tener visibilidad y control sobre las aplicaciones y sus funcionalidades en el trafico.
* Poder dar acceso a aplicaciones especificas y bloquear todo lo demas.
* Definir acceso de forma dinamica a aplicaciones y datos privilegiados con base a las membresias de grupos de usuarios.
* Definir acceso de forma dinamica el acceso desde equipos o grupos de equipos a aplicaciones y datos sensibles de usuarios o grupos de usuarios a dispositivos especificos.
* Capacidad para validar la identidad de un usuario mediante autenticacion
* Definicion dinamica de los recursos asociados a los datos confidenciales o a la aplicacion.
* Control de datos por tipo de archivo y contenido.
* Plataforma de segmentacion Zero Trust.
* Zonas de confianza.

## Capacidades del Zero Trust

El nucleo de cualquier arquitectura de seguridad de red Zero Trust es el Zero Trust segmentation platform, entonces tienes que escoger la solucion correcta. 

## Zero Trust Implementation

La implementación de un modelo de seguridad de red Zero Trust no requiere una revisión importante de la red y la infraestructura de seguridad de una organización.

Una arquitectura de diseño Zero Trust se puede implementar con solo modificaciones incrementales en la red existente, y la implementación puede ser completamente transparente para los usuarios. Las ventajas de este enfoque de implementación flexible y sin interrupciones incluyen minimizar el impacto potencial en las operaciones y poder distribuir la inversión y el esfuerzo de trabajo necesarios a lo largo del tiempo

1. Configure Listen-Only Mode: Para empezar, los equipos de seguridad pueden configurar una plataforma de segmentación Zero Trust en modo de solo escucha  para obtener una imagen detallada de los flujos de tráfico en toda la red, incluyendo dónde, cuándo y en qué medida usuarios específicos están utilizando aplicaciones y recursos de datos específicos.
2. Define Zero Trust Zones: Con un conocimiento detallado de los flujos de tráfico de red en el entorno, el siguiente paso es definir zonas de confianza y establecer gradualmente límites de confianza basados en el riesgo relativo o la sensibilidad de los datos involucrados. A continuación, deben configurar políticas de aplicación e inspección para poner en práctica de manera eficaz cada límite de confianza «en línea».  
3. Establish Zero Trust Zones: A continuación, los equipos de seguridad pueden establecer progresivamente zonas de confianza y límites para otros segmentos del entorno informático en función de su grado relativo de riesgo. 
4. Implement at Major Access Points: Los principios y conceptos de Zero Trust deben implementarse en los principales puntos de acceso a Internet. Los equipos de seguridad tendrán que sustituir o ampliar los dispositivos de seguridad de red heredados por una plataforma de segmentación Zero Trust en esta fase de implementación para obtener las capacidades y ventajas de un modelo de seguridad Zero Trust.


