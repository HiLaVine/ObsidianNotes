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

### Principios principales del Zero Trust



