# Azure-Guide
 Guía realizada como parte del curso para la certificación de Azure Fundamentals


## Módulo #2: Conceptos Fundamentales de Azure.
  - **Alta disponibilidad:** según el nivel del servicio, las aplicaciones en la nube pueden funcionar 24/7.
  
  - **Escalabilidad vertical:** la RAM o la CPU pueden aumentarse.
  - **Escalabilidad horizontal:** se incrementa la capacidad de computo de algo ya existente (como si fuera en paralelo).
  - **Elasticidad:** el que tanto puede estirarse un recurso. En este caso, siempre hay de donde agarrar.
  - **Agilidad:** El que tan rápido se puede responder a la necesidad que se tiene.
  - **Tolerancia a fallo:** se tienen respaldos de tu información, y geodistribución en la nube para que en caso de falla los         datos sgan seguros.
  - **CapEx (Capital expenditure):** dinero destinado para infraestructura física y su mantenimiento.
  - **OpEx (Operative expenditure):** dinero usado para seguir operando.
  - **Nube pública:** son servicios que están disponibles para cualquier persona.
  - **Nube privada:** recursos informáticos o información de una propiedad privada.
  - **Nube híbrida:** es una mezcla entre las nubes pública y privada.
  - **Infraestructura as a service (IaaS):** modelo en el cual solo el proveedor se encarga del hardware.
  - **Platform as a service (PaaS):** modelo en que el proveedor proporciona los recursos virtuales y el inquilino las              aplicaciones.
  - **Software as a Service (Saas):** el proveedor se encarga de las aplicaciones, el inquilino de los datos.
  - **Recursos:** elementos administrables.
  - **Grupo de recursos:** contenedor que incluye los recursos relacionados a una solución.
  - **Gobernanza:** reglas y directivas sobre los recursos de la organización.
  - **Nivel de servicio (SLA):** porcentaje de disponibilidad y rendimiento de los recursos.
  - **Azure:** servicio de nube de Microsoft que entrega servicios informáticos a través de internet.
  - **Cómputo en la nube:** servicios de computo entregados por internet.
  - **Categorías de Azure**
      - **Compute:** proporciona servicios de cómputo o procesamiento bajo demanda. Ejemplos; máquinas virtuales, kubernetes,       Azure functions.
      - **Network:** proporciona servicios de red para conectar recursos con el mundo exterior. Ejemplo: Azure Virtual             Network.
      - **Storage:** proporciona servicios de almacenamiento de archivos y objetos.
      - **Database:** proporciona servicios de base de datos.
      - **Internet of things:** proporciona servicios de IoT para conectar y recibir información de los dispositivos.
      - **Big data:** proporciona servicios para el procesamiento y análisis de información.
      - **Inteligencia artificial:** proporciona servicios de aprendizaje automático.
      - **DevOps:** ayuda a los equipos de desarrollo de software a automatizar y eficientizar sus procesos.
  
## Módulo #3: Descripción de los componentes principales de la arquitectura de Azure.

### Introducción a las suscripciones, los grupos de administración y los recursos de Azure
 ![image](https://user-images.githubusercontent.com/74509297/125119420-b5945900-e0b6-11eb-806c-21399e885ae1.png)


  - **Recursos:** son servicios que puede crear. Ejemplos; máquinas virtuales, almacenamiento o bases de datos SQL.
  
  - **Grupos de recursos:** actúan como contenedor lógico en el que se implementan y administran recursos de Azure como aplicaciones web, bases de datos o almacenamiento.
  - **Suscripciones:** agrupan las cuentas de usuario y los recursos que estas han creado. Cada suscripción tiene un límite o cuota respecto a los recursos que pueden usar. 
  - **Grupos de administración:** ayudan a administrar el acceso, directivas y el cumplimiento de varias suscripciones. Todas las suscripciones de un grupo de administración heredan las condiciones que tiene el grupo de administración.
  
### Zonas de disponibilidad, pares de regiones y regiones de Azure
 - **Región:** área geográfica que contiene al menos un centro de datos.
 - **Zona de disponibilidad:** centros separados físicamente dentro de una región de Azure, constan de uno o varios centros de datos con su infraestructura necesaria.
   - **Servicios de zona:** sirven para anclar un recurso a una zona específica.
   - **Servicios de redundancia de zona:** para replicar automáticamente datos en las zonas.

### Recursos de Azure y Azure Resource Manager. 
 - **Recurso:** elemento administrable, como máquinas virtuales, cuentas de almacenamiento, aplicaciones web, bases de datos, etc.
 - **Grupo de recursos:** es un contenedor para recursos implementados en Azure. 
 - **Agrupación lógica:** los recursos se ordenan de tipo, ubicación similar o uso, con lo cual le proporciona orden y organización a los recursos creados.
 - **Ciclo de vida:** al eliminarse un grupo de recursos, también se eliminan los recursos que contenía. Organizarlos de esta forma es útil para experimentar y descartar.
 - **Autorización:** puede limitar el acceso para permitir solo lo necesario.
 
 **Azure Resource Manager**
 Es el servicio de implementación y administración para Azure. Permite crear, actualizar y eliminar los recursos de una cuenta. Con esto puede controlar el acceso, los bloqueos, y las etiquetas para proteger y organizar los recursos luego de implementarlos.
 ![image](https://user-images.githubusercontent.com/74509297/125124039-19ba1b80-e0bd-11eb-97a9-6ed584d29c24.png)

Ventajas:
 - Administrar la infraestructura mediante plantillas en vez de scripts.
 - Controlar, implementar, administrar o supervisar en grupo.
 - Controlar el acceso a los servicios.
 
### Suscripciones y grupos de administración de Azure
El uso de Azure requiere de una suscripción, esta le proporciona acceso autenticado y autorizado a los servicios y productos de Azure, además le permite aprovisionar los recursos.
Una cuenta puede tener varias suscripciones con distintos modelos de facturación. Hay 2 tipos de límites de suscripción a utilizar.
 - **Límite de facturación**
 - **Límite de control de acceso**

- **App Service:** es un servicio basado en HTTP que permite crear y hospedar sitios web, aplicaciones, API, etc. sin necesidad de administrar la infraestructura. 
- **Azure Marketplace:** es una tienda en línea que hospeda aplicaciones certificadas y optimizadas para ejecutarse en Azure. Abarcan cosas como inteligencia artificial o machine learning

 ## Módulo #4: Exploración de los servicios de Azure Compute.
 
 **Azure Compute:** es un servicio de informática para ejecutar aplicaciones basadas en la nube. Los servicios mas destacados son:
  - **Azure Virtual Machines:** son emulaciones de software de equipos físicos. Virtual Machines proporciona infraestructura como servicio y puede usarse de maneras diferentes. 
      - **Conjunto de escalado de máquinas virtuales:** son un recurso que puede usarse para implementar y administrar un conjunto de VM idénticas.
      - Las VM son una opción ideal cuando se necesita; un control total sobre el sistema operativo, la capacidad para ejecutar software personalizado o para usar configuraciones de hospedaje personalizadas.
  - **Azure container instances:** los contenedores y kubernetes son entornos de aplicación ligeros y virtualizados. Están diseñados para crearse, escalarse horizontalmente y detenerse dinámicamente de forma rápida.
    - Los contenedores son un entorno de virtualización ligeros diseñados para crearse, escalarse horizontalmente y detenerse. Hay 2 tipos, Azure Container Instances y Azure Kubernetes Service.
  - **Azure App Service:** sirve para compilar, implementar y escalar de forma rápida aplicaciones de API, móviles y web de nivel empresarial que puedan ejecutarse en cualquier plataforma. 
  - **Azure Functions:** es utilizada cuando la unica preocupación es el código que ejecuta el servicio y no la infraestructura o plataforma subyacente. 

 ## Módulo #5: Exploración de los servicios de red de Azure.
 Las redes virtuales le permiten a los recursos de Azure comunicarse entre sí, con usuarios de internet y con los equipos del cliente. *Es un conjunto de recursos que se vincula con otros recursos de Azure.*
 Las redes de Azure proporcionan las siguientes funcionalidades:
  - **Aislamiento y segmentación:** Virtual Network permite crear varias redes virtuales aisladas. También se puede configurar la red virtual para que use un servidor DNS interno o externo.
  - **Comunicación con internet:** una VM puede conectarse a internet de forma predeterminada. Puede habilitar las comunicaciones entrantes desde internet si define una IP pública.
  - **Comunicación entre recursos de Azure:** se puede hacer de dos maneras:
    - *Redes virtuales:* pueden conectarse con distintos recursos de Azure como App Service Environment o Azure Kubernetes Service.
    - *Puntos de conexión de servicio:* con esto puede conectarse con cuentas de almacenamiento y bases de datos SQL de Azure.
  - **Comunicación con los recursos locales:** las redes virtuales de Azure permiten vincular entre sí los recursos del entorno local y dentro de la suscripción de Azure.
    - *Redes Privadas virtuales de punto a sitio:* El equipo cliente inicia una conexión VPN cifrada para conectar ese equipo a la red virtual de Azure.
    - *Redes virtuales privadas de sitio a sitio:* vinculan un dispositivo o puerta de enlace de VPN local con la puerta de enlace de VPN de Azure en una red virtual. 
    - *Azure ExpressRoute:* para los entornos en donde se requiere de mayor ancho de banda o de seguridad. ExpressRoute proporciona una conectividad privada dedicada de Azure.
  - **Enrutamiento del tráfico de red:** de forma predeterminada Azure enruta el tráfico entre las subredes de todas las redes virtuales conectadas, las redes locales e Internet.
    - *Tablas de rutas:* permite definir reglas para dirigir el tráfico.
    - *Protocolo de puerta de enlace de borde (BGP) :* funciona con puertas de enlace de VPN de Azure o con ExpressRoute para propagar las rutas BGP locales a través de las redes virtuales de Azure.
  - **Filtrado del tráfico de red:** permiten filtrar el tráfico entre las subredes mediante los métodos siguientes:
    - *Grupos de seguridad de red:* es un recurso de Azure que puede contener varias reglas de seguridad de entrada y salida.
    - *Aplicaciones virtuales de red:* una aplicación virtual de red es una máquina virtual especializada que se puede comparar con un dispositivo de red protegido, ejerce una función de red determinada, como ejecutar un firewall o realizar la optimización de la red de área extensa (WAN).
  - **Conexión de redes virtuales:** Puede vincular redes virtuales entre sí mediante el emparejamiento de red virtual, esto permite que los recursos de cada red virtual se comuniquen entre sí. 

### Creación de una red virtual. 
Para crear una red virtual, se configuran algunas opciones básicas. 
- **Nombre de la red**
- **Espacio de direcciones:** se define el espacio de direcciones internas con el formato de Enrutamiento de interdominios sin clases (CIDR). Este espacio de direcciones debe ser único dentro de la suscripción y de cualquier otra red a la que se conecte.
- **Suscripción:** Solo si tiene varias suscripciones a elegir.
- **Grupo de recursos:** una red virtual debe existir dentro de un grupo de recursos, puede seleccionar uno existente o crear otro.
- **Ubicación**
- **Subred:** puede crear una o varias subredes que dividirán el espacio de direcciones de la red virtual. El enrutamiento entre las subredes dependerá de las rutas de tráfico predeterminadas.
- **Protección contra DDoS**
- **Puntos de conexión de servicio**

Después de crear una red virtual se tienen mas opciones para configurar.
- **Grupo de seguridad de red**
- **Tabla de rutas**
- **Espacios de direcciones**
- **Dispositivos conectados**
- **Subredes**
- **Emparejamientos**

Las redes virtuales son mecanismos eficaces y muy configurables para conectar las entidades de Azure. Puede conectar los recursos de Azure entre sí o a los recursos del entorno local. Puede aislar, filtrar y enrutar el tráfico de red. Azure le permite aumentar la seguridad donde considere que es necesario.

### Aspectos básicos de Azure ExpressRoute
Permite ampliar las redes locales a la nube de Microsoft mediante una conexión privada con la ayuda de un proveedor de conectividad. Hay 2 niveles:
- **Nivel 2 (L2):**  se trata del nivel de vínculo de datos, que proporciona una comunicación de nodo a nodo entre dos nodos de la misma red.
- **Nivel 3 (L3):** se trata del nivel de red, que proporciona el direccionamiento y enrutamiento entre los nodos de una red de varios nodos.

** Características y ventajas**
- Conectividad de nivel 3 entre su red local y Microsoft Cloud a través de un proveedor de conectividad. La conectividad puede ser desde una red de conectividad universal (IP VPN), una red Ethernet de punto a punto, o una conexión cruzada virtual a través de un intercambio de Ethernet.
- Conectividad de servicios en la nube de Microsoft en todas las regiones dentro de la región geopolítica.
- Conectividad global a los servicios de Microsoft en todas las regiones con el complemento ExpressRoute Premium.
- Enrutamiento dinámico entre la red y Microsoft a través de BGP.
- Redundancia integrada en todas las ubicaciones de configuración entre pares para una mayor confiabilidad.
- El tiempo de actividad de conexión SLA.
- Compatibilidad con QoS de Skype para la empresa.

**Redundancia integrada**
Cada proveedor de conectividad usa dispositivos redundantes para garantizar que las conexiones establecidas con Microsoft tengan alta disponibilidad.

**Conectividad con los servicios en la nube de Microsoft**
ExpressRoute permite el acceso directo a los siguientes servicios en todas las regiones:
- Microsoft Office 365
- Microsoft Dynamics 365
- Servicios de proceso de Azure, como Azure Virtual Machines
- Servicios en la nube de Azure, como Azure Cosmos DB y Azure Storage

**Conectividad local con global reach de ExpressRoute**
Puede permitir que Global Reach de ExpressRoute intercambie datos entre los sitios locales si conecta los diferentes circuitos ExpressRoute. 

**Enrutamiento dinámico**
ExpressRoute usa el protocolo de enrutamiento Protocolo de puerta de enlace de borde (BGP). BGP se usa para intercambiar rutas entre las redes locales y los recursos que se ejecutan en Azure.

**Modelos conectividad de ExpressRoute**
ExpressRoute admite tres modelos que puede usar para conectar la red local con la nube de Microsoft:
- Ubicación de CloudExchange
- Conexión Ethernet de punto a punto
- Conexión universal
![image](https://user-images.githubusercontent.com/74509297/126248615-d30ef6a9-3816-4ba7-966a-747b06cfb318.png)

**Coubicación en un intercambio en la nube**
Los proveedores de coubicación pueden ofrecer conexiones de nivel 2 y nivel 3 entre la infraestructura, que puede encontrarse en las instalación de la coubicación, y la nube de Microsoft.

**Conexión Ethernet de punto a punto**
Las conexiones de punto a punto proporcionan conectividad de nivel 2 y nivel 3 entre el sitio local y Azure. Puede conectar sus oficinas o centros de datos a Azure mediante vínculos de punto a punto. 

**Redes universales**
Puede integrar la red de área extensa (WAN) con Azure si proporciona conexiones a las oficinas y los centros de datos. Con las conexiones universales, todos los proveedores de WAN ofrecen conectividad de nivel 3.

**Consideraciones sobre la seguridad**
ExpressRoute es una conexión privada de la infraestructura local a la infraestructura de Azure. Incluso si tiene una conexión ExpressRoute, las consultas de DNS, la comprobación de la lista de revocación de certificados y las solicitudes de Azure Content Delivery Network se siguen enviando a través de la red pública de Internet.

## Módulo #6: Exploración de los servicios de Azure Storage.
Azure Storage no es lo mismo que los servicios de base de datos de Azure. Azure Storage es un servicio que puede usar para almacenar archivos, mensajes, tablas y otros tipos de información.

### Aspectos básicos de Disk Storage
Proporciona discos para Azure Virtual Machines. Las aplicaciones y otros servicios pueden acceder a estos discos y usarlos cuando sea necesario, igual que se haría en escenarios locales, permite que los datos se almacenen de forma persistente y que se acceda a ellos desde un disco duro virtual conectado.

### Aspectos básicos de Azure Blob Storage
Azure Blob Storage es una solución de almacenamiento de objetos para la nube. Puede almacenar grandes cantidades de datos, como datos de texto o binario, es no estructurado, lo que significa que no hay ninguna restricción en cuanto a los tipos de datos que puede contener. Además puede administrar miles de cargas simultáneas, cantidades enormes de datos de vídeo, archivos de registro en constante crecimiento y es accesible desde cualquier lugar con conexión a Internet.
Los blobs no están limitados a formatos de archivo comunes. Un blob podría contener gigabytes de datos binarios transmitidos desde un instrumento científico, un mensaje cifrado para otra aplicación o datos en un formato personalizado para una aplicación que se está desarrollando.
Blob Storage resulta ideal para lo siguiente:
- Visualización de imágenes o documentos directamente en un explorador.
- Almacenamiento de archivos para acceso distribuido.
- Streaming de audio y vídeo.
- Almacenamiento de datos para copia de seguridad y restauración, recuperación ante desastres y archivado.
- Almacenamiento de datos para el análisis en local o en un servicio hospedado de Azure.
- Almacenamiento de hasta 8 TB de datos para máquinas virtuales.
Los blobs se almacenan en contenedores, lo que ayuda a organizar los blobs en función de sus necesidades empresariales.

### Aspectos básicos de Azure Files
Azure Files ofrece recursos compartidos de archivos totalmente administrados en la nube a los que se puede acceder mediante los protocolos del Bloque de mensajes del servidor y Network File System. Los recursos compartidos de Azure se pueden montar simultáneamente en implementaciones de Windows, Linux y macOS en la nube o locales. Las aplicaciones que se ejecutan en máquinas virtuales o servicios en la nube de Azure pueden montar un recurso compartido de almacenamiento de archivos para acceder a datos de archivos.
Use Azure Files para las siguientes situaciones:
- Muchas aplicaciones locales usan recursos compartidos de archivos. Azure Files facilita la migración de esas aplicaciones que comparten datos a Azure. Si monta el recurso compartido de archivos en la misma letra de unidad que usa la aplicación local, la parte de la aplicación que accede al recurso compartido de archivos debe funcionar con cambios mínimos, si los hay.
- Almacene archivos de configuración en un recurso compartido de archivos y acceda a ellos desde varias máquinas virtuales. Las herramientas y utilidades que usen varios desarrolladores de un grupo pueden almacenarse en un recurso compartido de archivos, lo que garantiza que todos los usuarios puedan encontrarlas y que utilizan la misma versión.
- Escriba datos en un recurso compartido de archivos y procese o analice los datos más adelante. Por ejemplo, puede que desee hacerlo con registros de diagnóstico, métricas y volcados de memoria.
Una cosa que distingue Azure Files de los archivos ubicados en un recurso compartido de archivos corporativo es que puede tener acceso a los archivos desde cualquier lugar del mundo mediante una dirección URL que apunte al archivo.

### Descripción de los niveles de acceso de blobs.

Azure Storage ofrece diferentes niveles de acceso para el almacenamiento de blobs, lo que le ayuda a almacenar datos de objetos de la manera más rentable. Entre los niveles de acceso disponibles se incluyen:
- Nivel de acceso frecuente: optimizado para almacenar datos a los que se accede con frecuencia (por ejemplo, imágenes para el sitio web).
- Nivel de acceso esporádico: optimizado para datos a los que se accede con poca frecuencia y que se almacenan al menos durante 30 días (por ejemplo, las facturas de los clientes).
- Nivel de acceso de archivo: conveniente para datos a los que raramente se accede y que se almacenan durante al menos 180 días con requisitos de latencia flexibles (por ejemplo, copias de seguridad a largo plazo).

Las siguientes consideraciones se aplican a los distintos niveles de acceso:
- Solo los niveles de acceso frecuente y esporádico se pueden establecer en el nivel de cuenta. El nivel de acceso de archivo no está disponible en el nivel de cuenta.
- Los niveles frecuente, esporádico y de archivo se pueden establecer en el nivel de blob durante la carga o después de esta.
- Los datos del nivel de acceso esporádico pueden tolerar una disponibilidad ligeramente inferior, pero aun así requieren una gran durabilidad, una latencia de recuperación y unas características de rendimiento similares a las de los datos de acceso frecuente. En el caso de los datos de acceso esporádico, un contrato de nivel de servicio (SLA) con una disponibilidad ligeramente inferior y unos costos de acceso mayores, en comparación con los datos de acceso frecuente, es aceptable a cambio de unos costos de almacenamiento menores.
- El almacenamiento de archivo almacena datos sin conexión y ofrece los menores costos de almacenamiento, pero los mayores costos de acceso y rehidratación de datos.


## Módulo #7: Exploración de los servicios de análisis y bases de datos de Azure.

### Azure Cosmos DB
Azure Cosmos DB es un servicio de base de datos de varios modelos distribuido globalmente, es compatible con los datos sin esquema, lo que le permite compilar aplicaciones "Always On" con una gran capacidad de respuesta para admitir datos en continuo cambio.

![image](https://user-images.githubusercontent.com/74509297/126828538-38b84b63-b0ad-4404-a460-2b8cd6b33dad.png)

### Azure SQL Database
SQL Database es una base de datos de alto rendimiento, confiable, totalmente administrada y segura. Azure SQL Database es un motor de base de datos de plataforma como servicio (PaaS). Controla la mayoría de las funciones de administración de bases de datos, como las actualizaciones, las aplicaciones de revisiones, las copias de seguridad y la supervisión, sin intervención del usuario.

**Migración**
Puede migrar las bases de datos existentes de SQL Server con un tiempo de inactividad mínimo mediante Azure Database Migration Service.


## Módulo #8: Elegir el mejor servicio de Azure IoT para su aplicación
## Módulo #9: Elija el mejor servicio de IA para sus necesidades
## Módulo #10: Elección de la mejor tecnología sin servidor de Azure para su escenario empresarial
## Módulo #11: Elección de las mejores herramientas para ayudar a que las organizaciones creen mejores soluciones


## Módulo #12: Elección de las mejores herramientas para administrar y configurar el entorno de Azure
## Módulo #13: Elección del mejor servicio de supervisión para visibilidad, información y mitigación de interrupciones
## Módulo #10:

Examen
Azure Monitor
