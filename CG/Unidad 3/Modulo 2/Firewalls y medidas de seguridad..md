Un firewall es un dispositivo de seguridad que monitorea el trafico de una red. 

Autoriza o bloquea el tráfico según el conjunto de reglas de seguridad. 

Port filtering (filtrar puertos)

Se usa para bloquear o permitir cierto numero de puertos y limitar la comunicación indeseada. 

## Tipos de firewalls

* Hardware firewall: es la defensa básica mas básica contra amenazas.  Este inspecciona cada paquete de datos antes de autorizar su entrada a la red. 
* Software firewall: funciona igual que un hardware firewall pero no es un dispositivo físico.  
* Cloud Firewall: los proveedores de servicios en la nube ofrecen firewall como servicio, FaaS. Son software firewalls pero alojados en un CSP. 

### Stateful Firewall

Es una clase de firewall que hace un seguimiento de la información que pasa a través de el y filtra previamente las amenazas. Busca:
- caracteristicas y comportamientos sospechosos del trafico y evita que entren en la red. 

### Stateless firewall

Opera basado en reglas predefinidas y no hace un seguimiento de la información que proviene de los paquetes de datos. 

- Solo actúa en base a las reglas preconfiguradas 

### NGFW

Es un firewall de ultima generación, ya que ofrece mas seguridad que un cortafuegos stateful. No solo realiza una inspección stateful del trafico entrante y saliente, tambien realiza funciones mas profundas como la inspeccion profunda de paquetes y proteccion contra intrussiones. Algunos se conectan a servicios basados en nube de intelifencia de amenazass. Capa de la 3 a la 7