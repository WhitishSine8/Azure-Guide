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

### Azure Database for PostgreSQL
Es un servicio de base de datos relacional en la nube. Ofrece las siguientes ventajas:
 - Alta disponibilidad integrada en comparación con los recursos locales.
 - Precios sencillos y flexibles.
 - Escalado o reducción vertical según sea necesario, en cuestión de segundos. 
 - Copias de seguridad automáticas ajustables y restauración a un momento dado durante un máximo de 35 días.
 - Seguridad y cumplimiento de nivel empresarial para proteger la información confidencial en reposo y en movimiento.

Azure Database for PostgreSQL está disponible en dos opciones de implementación: Servidor único e Hiperescala (Citus).

**Servidor único**
La opción de implementación Un solo servidor ofrece:

- Alta disponibilidad integrada sin coste adicional (contrato de nivel de servicio del 99,99 %).
- Rendimiento predecible y precios de pago por uso inclusivos.
- Escalado vertical según sea necesario, en cuestión de segundos.
- Supervisión y alertas para evaluar el servidor.
- Seguridad y cumplimiento de nivel empresarial.
- Capacidad de protección de información confidencial en reposo y en movimiento.
- Copias de seguridad automáticas y restauración a un momento dado durante un máximo de 35 días.

**Hiperescala (Citus)**
Escala horizontalmente las consultas entre varias máquinas mediante el particionamiento. Su motor de consultas paraleliza las consultas SQL entrantes en estos servidores para agilizar las respuestas en conjuntos de datos grandes.

### Azure SQL Managed Instance
Es un servicio de datos en la nube escalable que proporciona la mayor compatibilidad con el motor de base de datos de SQL Server con todas las ventajas de una plataforma como servicio totalmente administrada. En función de su escenario, Azure SQL Managed Instance podría ofrecer más opciones para sus necesidades de base de datos. Es un motor de base de datos de plataforma como servicio (PaaS).

**Migración**
Azure SQL Managed Instance facilita la migración de los datos locales en SQL Server a la nube con Azure Database Migration Service (DMS) o copias de seguridad y restauración nativas.
![image](https://user-images.githubusercontent.com/74509297/126855120-5d12befd-fcb2-4304-8dbb-a0ea142bb47d.png)

### Exploración de análisis y macrodatos.
Microsoft Azure admite una amplia gama de tecnologías y servicios para proporcionar soluciones de macrodatos y análisis, como Azure Synapse Analytics, Azure HDInsight, Azure Databricks y Azure Data Lake Analytics.
 - **Azure Synapse Analytics:** es un servicio de análisis ilimitado que reúne el almacenamiento de datos empresariales y el análisis de macrodatos.
 - **Azure HDInsight:** es un servicio de análisis de código abierto totalmente administrado para empresas. Puede ejecutar marcos de código abierto populares y crear tipos de clúster. También admite una amplia gama de escenarios, como la extracción, la transformación y la carga de datos (ETL), el almacenamiento de datos, el aprendizaje automático e IoT.
 - **Azure Databricks:** le ayuda a descubrir información de todos los datos y a crear soluciones de inteligencia artificial.
 - **Análisis con Azure Data Lake:** es un servicio de trabajos de análisis a petición que simplifica los macrodatos, escribirá consultas para transformar los datos y extraer ideas valiosas.


## Módulo #8: Elegir el mejor servicio de Azure IoT para su aplicación

### Azure IoT Hub
Es un servicio administrado hospedado en la nube que actúa como centro de mensajes centralizado para la comunicación bidireccional entre la aplicación de IoT y los dispositivos que administra. Admite las comunicaciones desde el dispositivo a la nube y desde la nube al dispositivo. Una vez que un centro de IoT recibe los mensajes de un dispositivo, puede enrutarlos a otros servicios de Azure. IoT Hub permite ordenar y controlar.

### Azure IoT Central
Se basa en IoT Hub y agrega un panel que le permite conectar, supervisar y administrar sus dispositivos de IoT. Una parte clave de IoT Central es el uso de las plantillas de dispositivo. Las plantillas de dispositivo permiten conectar un dispositivo sin programación en el lado del servicio.

### Azure Sphere
Crea una solución de IoT de un extremo a otro de alta seguridad para los clientes que lo abarca todo, desde el hardware y el sistema operativo del dispositivo hasta el método seguro para enviar mensajes desde el dispositivo al centro de mensajes.
Consta de 3 partes:
 - La primera parte es la unidad de microcontrolador (MCU) de Azure Sphere, que se encarga de procesar el sistema operativo y las señales de los sensores conectados.
 - La segunda parte es un sistema operativo (SO) Linux personalizado, que controla la comunicación con el servicio de seguridad y puede ejecutar el software del proveedor.
 - La tercera parte es el servicio de seguridad de Azure Sphere. Su trabajo es asegurarse de que el dispositivo no se ha puesto en peligro de forma malintencionada.

### Análisis de los criterios de decisión
Cuando la seguridad es una cuestión fundamental en el diseño del producto, la mejor opción de producto es Azure Sphere, que proporciona una solución completa de un extremo a otro para dispositivos de IoT.
Azure Sphere garantiza un canal seguro de comunicación entre el dispositivo y Azure mediante el control de todo, desde el hardware hasta el sistema operativo y el proceso de autenticación.


## Módulo #9: Elija el mejor servicio de IA para sus necesidades
La IA es una clasificación amplia de la informática que permite que un sistema de software perciba su entorno y tome medidas que maximicen sus probabilidades de éxito a la hora de lograr sus objetivos.
El objetivo de la IA es crear un sistema de software que pueda adaptarse o aprender algo por sí mismo sin estar programado explícitamente para hacerlo.

### Azure Machine Learning

Elija Azure Machine Learning cuando los científicos de datos necesiten un control completo sobre el diseño y el entrenamiento de un algoritmo con sus propios datos.
Es una plataforma para realizar predicciones, con la que se puede realizar lo siguiente:
 - Crear un proceso que defina cómo obtener los datos, cómo tratar los datos que faltan o que son incorrectos, cómo dividir los datos en un conjunto de entrenamiento o de pruebas y cómo enviar los datos al proceso de entrenamiento.
 - Entrenar y evaluar modelos predictivos mediante herramientas y lenguajes de programación conocidos por los científicos de datos.
 - Crear canalizaciones que definan dónde y cuándo ejecutar los experimentos de proceso intensivo necesarios para puntuar los algoritmos en función de los datos de entrenamiento y de prueba.
 - Implementar el algoritmo de mejor rendimiento como una API en un punto de conexión para que otras aplicaciones puedan consumirlo en tiempo real.

### Azure Cognitive Services

Use Azure Cognitive Services para solucionar problemas generales, como el análisis de texto para detectar opiniones o el análisis de imágenes para reconocer objetos o caras.
Azure Cognitive Services proporciona modelos de aprendizaje automático creados previamente que permiten a las aplicaciones ver, oír, hablar, comprender e incluso empezar a pensar. Azure Cognitive Services se puede dividir en las categorías siguientes:
- Servicios de lenguaje: permita que las aplicaciones procesen lenguaje natural con scripts precompilados, evalúen opiniones y aprendan a reconocer lo que quieren los usuarios.
- Servicios de voz: convierta voz en texto y texto en voz de sonido natural. Traduzca de un idioma a otro y habilite el reconocimiento y la verificación del hablante.
- Servicios de visión: agregue capacidades de reconocimiento e identificación al analizar imágenes, vídeos y otro contenido visual.
- Servicios de decisión: agregue recomendaciones personalizadas para cada usuario que mejoren automáticamente cada vez que se usen, modere contenido para supervisar y quitar el contenido ofensivo o arriesgado y detecte anomalías en los datos de series temporales.

### Azure Bot Service (y Bot Framework)
Son plataformas para crear agentes virtuales que comprenden y responden a preguntas como un ser humano. Azure Bot Service se diferencia de Azure Machine Learning y Azure Cognitive Services en que tiene un caso de uso concreto: *crear un agente virtual que pueda comunicarse de forma inteligente con los usuarios.*
Los bots se pueden usar para convertir tareas sencillas y repetitivas, como tomar una reserva de cena o recopilar información de perfil, en sistemas automatizados que ya no requieran la intervención humana directa. Los usuarios conversan con un bot mediante texto, tarjetas interactivas y voz.

### Análisis de los criterios de decisión
**Azure Bot Service**
Use Azure Bot Service cuando necesite crear un agente virtual para interactuar con los usuarios mediante el lenguaje natural. 
Antes de entrar de pleno en la creación de una experiencia de chat personalizada con Bot Service, puede que sea mejor buscar soluciones precompiladas sin código que abarquen los escenarios habituales.

**Azure Cognitive Services**
Use Azure Cognitive Services cuando necesite realizar tareas de uso general, como la conversión de voz en texto, la integración con búsquedas o la identificación de objetos en una imagen. 

El servicio Azure Cognitive Services Personalizer supervisa las acciones de los usuarios en una aplicación. Puede usar Personalizer para predecir su comportamiento y proporcionar experiencias relevantes a medida que identifique patrones de uso.

Elija Azure Machine Learning cuando necesite analizar datos para predecir resultados futuros.

Use Azure Machine Learning para obtener la máxima flexibilidad.


## Módulo #10: Elección de la mejor tecnología sin servidor de Azure para su escenario empresarial
**Informática sin servidor:** es un término usado para describir un entorno de ejecución que se configura y administra de manera automática. Es un entorno de ejecución hospedado en la nube que ejecuta código, pero abstrae el entorno de hospedaje subyacente.

La idea clave es que el cliente no es responsable de la configuración o el mantenimiento del servidor. El proveedor de la nube se encarga de todo el mantenimiento y el escalado. El cliente crea una instancia del servicio y, después, agrega su código. Suele utilizarse para controlar los escenarios de back-end.

### Azure Functions
Con este servicio, puede hospedar un único método o función mediante un lenguaje de programación popular en la nube que se ejectura en respuesta a un evento. Se escala automáticamente.
La solución Azure Functions es ideal si le preocupa solo el código que ejecuta el servicio y no la infraestructura o la plataforma subyacente.

### Azure Logic Apps
Es una plataforma de desarrollo de poco (o sin) código hospedada como un servicio en la nube. 
Está diseñado en un entorno web y puede ejectuar una lógica que los servicios de Azure desencadenan sin escribir código. 

### Diferencias entre Azure Functions y Azure Logic Apps
Puede llamar a Azure Functions desde Azure Logic Apps y viceversa.
Azure Functions es un servicio informático sin servidor, y Azure Logic Apps está diseñado para ser un servicio de orquestación sin servidor.


## Módulo #11: Elección de las mejores herramientas para ayudar a que las organizaciones creen mejores soluciones

### Azure DevOps Services 
Es un conjunto de servicios que aborda cada fase del ciclo de vida de desarrollo de software:
 - **Azure Repos** es un repositorio de código fuente centralizado en el que los profesionales de desarrollo de software, ingeniería DevOps y documentación pueden publicar su código para su revisión y colaboración.
 - **Azure Boards** es un conjunto de administración de proyectos ágil que incluye paneles Kanban, informes, ideas de seguimiento y trabajo desde epopeyas de alto nivel hasta incidencias y elementos de trabajo.
 - **Azure Pipelines** es una herramienta de automatización de canalizaciones de CI/CD.
 - **Azure Artifacts** es un repositorio para hospedar artefactos, como código fuente compilado, que se puede incluir en los pasos de canalización de pruebas o de implementación.
 - **Azure Test Plans** es una herramienta de pruebas automatizadas que se puede usar en una canalización de CI/CD para garantizar la calidad antes de publicar una versión de software.

### Azure DevTest Labs
Proporciona un medio automatizado para administrar el proceso de compilación, configuración y anulación de máquinas virtuales que contienen las compilaciones de los proyectos de software.
Cualquier cosa que se pueda implementar en Azure a través de una plantilla de Resource Manager se puede aprovisionar a través de DevTest Labs.
Si su objetivo es automatizar la creación y la administración de un entorno de laboratorio de pruebas, considere la posibilidad de elegir Azure DevTest Labs. De las tres herramientas y servicios que hemos descrito, es el único que ofrece esta funcionalidad.


## Módulo #12: Elección de las mejores herramientas para administrar y configurar el entorno de Azure
Mediante las herramientas de administración de Azure, los administradores y desarrolladores pueden interactuar con el entorno de nube para realizar tareas como:

 - Implementar decenas o cientos de recursos a la vez.
 - Configurar servicios individuales mediante programación.
 - Ver informes enriquecidos relativos al uso, el mantenimiento, los costos y mucho más.

Hay dos categorías amplias de herramientas de administración: herramientas visuales y herramientas basadas en código.
 - Herramientas visuales: proporcionan acceso completo y visualmente sencillo a toda la funcionalidad de Azure. Sin embargo son menos útiles para configurar una gran implementación de recursos con interdependencias y opciones de configuración.
 - Herramienta basada en código: se usa para intentar instalar y configurar rápidamente los recursos de Azure. 

### Infraestructura como código
 - Código imperativo: detalla cada uno de los pasos que debe realizarse para lograr un resultado deseado.
 - Código declarativo: detalla un resultado deseado, y el intérprete debe luego decidir cual es la mejor forma de lograr este resultado.

**Azure Portal** 
Dispone de una UI gráfica sencilla en la que se pueden ver todos los servicios que se están usando, crear servicios nuevos, configurar los servicios y ver informes. Con Azure Portal puede realizar la mayoría de las acciones administrativas.
Azure Portal es un lugar excelente para que los principiantes obtengan información sobre Azure y configuren sus primeros recursos.

**Azure Mobile App**
Le permite acceder a los recursos de Azure desde iOS y Android cuando no tiene el equipo a mano.
 - Supervisar el mantenimiento y el estado de sus recursos de Azure.
 - Consultar alertas, diagnosticar y corregir problemas rápidamente, reiniciar una aplicación web o una máquina virtual (VM).
 - Ejecutar comandos de la CLI de Azure o de Azure PowerShell para administrar los recursos de Azure.

**Azure PowerShell**
Es un shell que permite a los desarrolladores, y profesionales de TI y DevOps ejecutar comandos denominados cmdlets o command-lets.
 - La configuración de rutinas, la anulación y el mantenimiento de un único recurso o de varios recursos conectados.
 - La implementación de una infraestructura completa, que puede contener decenas o cientos de recursos, de código imperativo.
Azure PowerShell y la CLI de Azure son herramientas de administración de Azure que le permiten obtener rápidamente la dirección IP de una máquina virtual (VM) que ha implementado, reiniciar una VM o escalar una aplicación. 

**Azure CLI**
La CLI de Azure le permite usar Bash para ejecutar tareas puntuales en Azure.

**Plantillas de ARM**
Al usar las plantillas de Azure Resource Manager (ARM), puede describir los recursos que quiere usar en un formato JSON declarativo.
Definen los requisitos de infraestructura de la aplicación para implementaciones que se repiten. 
Las plantillas de Resource Manager son la mejor opción de infraestructura como código para configurar de manera rápida y fiable toda la infraestructura en la nube de forma declarativa.


## Módulo #13: Elección del mejor servicio de supervisión para visibilidad, información y mitigación de interrupciones

###Azure Advisor
Elija Azure Advisor si quiere realizar un análisis de los recursos implementados.
Azure Advisor es la opción de producto adecuada para ayudar a optimizar y entender mejor su gasto y su postura de seguridad en la nube. 
Evalúa los recursos de Azure y hace recomendaciones que contribuyen a mejorar la confiabilidad, la seguridad y el rendimiento, lograr la excelencia operativa y reducir los costos.
El panel Advisor de Azure Portal muestra recomendaciones personalizadas para todas las suscripciones. Las recomendaciones se dividen en cinco categorías:
 - Confiabilidad: se usa para garantizar y mejorar la continuidad de las aplicaciones críticas para la empresa.
 - Seguridad: se usa para detectar amenazas y vulnerabilidades que podrían dar lugar a infracciones de seguridad.
 - Rendimiento: se usa para mejorar la velocidad de las aplicaciones.
 - Costos: se usan para optimizar y reducir el gasto general de Azure.
 - Excelencia operativa: se usa para conseguir procedimientos recomendados de eficiencia en procesos y flujos de trabajo, manejabilidad de los recursos e implementación.


### Azure Monitor
Elija Azure Monitor si quiere medir eventos personalizados y otros datos de telemetría recopilados, además de configurar alertas de eventos clave relacionados con sus recursos específicos.
Es una plataforma que permite recopilar, analizar y mostrar datos, así como llevar a cabo acciones en función de las métricas y los datos registrados en todo el entorno local y de Azure.

![image](https://user-images.githubusercontent.com/74509297/127340460-2a1cf982-1d5e-4239-bcd9-a1200a734fa2.png)

 - A la izquierda aparece una lista de los orígenes de los datos de métricas y registros,
 - En el centro, puede ver cómo se almacenan los datos de registro y métricas en los repositorios centrales.
 - A la derecha, los datos se usan de diversas formas.
Puede usar los datos para ayudarle a reaccionar ante eventos críticos en tiempo real gracias a las alertas enviadas a los equipos por SMS, correo electrónico, etc.

### Azure Service Health
Si quiere mantener un control de Azure, especialmente de los servicios y regiones de los que dependa, debe elegir Azure Service Health. 
Proporciona una vista personalizada del estado de los servicios, regiones y recursos de Azure en los que se basa su infraestructura. Service Health le ayuda a supervisar varios tipos de eventos:
 - Los problemas de servicio son problemas de Azure, como las interrupciones, que le afectan en este momento. 
 - Mantenimiento planeado: este tipo de eventos pueden afectar a la disponibilidad. P
 - Avisos de estado: son problemas que exigen actuar para evitar la interrupción del servicio, e incluyen retiradas del servicio y cambios importantes. Los avisos de estado se anuncian con mucha antelación para que pueda planear su respuesta.


## Módulo #14: Protección frente a amenazas de seguridad en Azure.

### Azure Security Center
Es un servicio de supervisión que proporciona visibilidad del nivel de seguridad en todos los servicios, tanto en Azure como en el entorno local.
**Nivel de seguridad:** se refiere a las directivas y a los controles de ciberseguridad, así como a la predicción, la prevención y la respuesta a las amenazas de seguridad.
Security Center puede:
 - Supervisar la configuración de seguridad en las cargas de trabajo locales y en la nube.
 - Aplicar automáticamente la configuración de seguridad necesaria a los nuevos recursos a medida que se publican en línea.
 - Proporcionar recomendaciones de seguridad basadas en las configuraciones, los recursos y las redes actuales.
 - Supervisar de forma continua los recursos y realizar valoraciones de seguridad automáticas para identificar posibles vulnerabilidades antes de que alguien las aproveche.
 - Usar el aprendizaje automático para detectar y bloquear la instalación de malware en las máquinas virtuales (VM) y otros recursos. 
 - Detectar y analizar posibles ataques entrantes e investigar amenazas y otras actividades posteriores a una brecha que pudieran haberse producido.
 - Proporcionar control de acceso Just-in-Time a los puertos de red. 

**Puntuación de seguridad:** es una medida de nivel de seguridad de una organización. Se basa en controles de seguridad, o en grupos de recomendaciones de seguridad relacionadas. La puntuación de seguridad ayuda a:
 - Notificar el estado actual del nivel de seguridad de la organización.
 - Mejorar el nivel de seguridad al proporcionar detectabilidad, visibilidad, orientación y control.
 - Comparar con los puntos de referencia y establecer indicadores clave de rendimiento (KPI).

**Protección contra amenazas**
Security Center incluye funciones avanzadas de defensa en la nube para máquinas virtuales, seguridad de red e integridad de archivos:
 - Acceso de máquina virtual Just-In-Time
 - Controles de aplicación adaptables
 - Protección de red adaptable
 - Supervisión de la integridad de los archivos

### Azure Sentinel
Azure Sentinel permite:
 - **Recopilar datos en la nube a gran escala:** Recopile datos de todos los usuarios, dispositivos, aplicaciones e infraestructura, tanto locales como de varias nubes.
 - **Detectar amenazas no detectadas anteriormente:** Minimice los falsos positivos mediante el análisis exhaustivo y la inteligencia sobre amenazas de Microsoft.
 - **Investigar amenazas con inteligencia artificial:** Examine actividades sospechosas a gran escala y aproveche años de experiencia de ciberseguridad de Microsoft.
 - **Responder a incidentes rápidamente:** Use la orquestación integrada y la automatización de tareas comunes.
 - **Conexión de soluciones de Microsoft:** los conectores proporcionan integración en tiempo real para servicios como las soluciones de Protección contra amenazas de Microsoft, orígenes de Microsoft 365 (incluido Office 365), Azure Active Directory y Firewall de Windows Defender.
 - **Conexión con otros servicios y soluciones:** Hay conectores disponibles para servicios y soluciones comunes que no son de Microsoft, incluidos AWS CloudTrail, Citrix Analytics (Security), Sophos XG Firewall, VMware Carbon Black Cloud y Okta SSO.
 - **Conexión con orígenes de datos estándar del sector:** Azure Sentinel admite datos de otros orígenes que usan el estándar de mensajería Formato de evento común (CEF), Syslog o la API REST.

**Análisis integrados:** usan plantillas diseñadas por el equipo de expertos y analistas de seguridad de Microsoft que se basan en amenazas conocidas, vectores de ataque comunes y cadenas de escalado de actividades sospechosas.
**Análisis personalizados:** son reglas que se crean para buscar criterios concretos en el entorno.

### Azure Key Vault
Es un servicio en la nube centralizado para almacenar los secretos de la aplicación en una única ubicación central, puede ayudar a:
 - Administrar contraseñas, tokens, certificados, etc.
 - Administrar claves de cifrado.
 - Administrar certificados SSL/TLS
 - Almancenar secretos respaldados por módulos de seguridad de hardware.

**Ventajas**
 - Secretos de aplicación centralizados
 - Secretos y claves almacenados de forma segura
 - Supervisión y control de acceso
 - Administración simplificada de secretos de aplicación
 - Integración con otros servicios de Azure

### Azure Dedicated Host

Azure Dedicated Host:

 - Ofrece visibilidad y control sobre la infraestructura de servidor que ejecuta las máquinas virtuales de Azure.
 - Ayuda a satisfacer requisitos de cumplimiento mediante la implementación de las cargas de trabajo en un servidor aislado.
 - Permite elegir el número de procesadores, capacidades de servidor, series de máquinas virtuales y tamaños de máquina virtual dentro del mismo host.


## Módulo #15: Conectividad de red segura en Azure
**Defensa en profundidad:** su objetivo es proteger la información y evitar que personas no autoriazadas a acceder a ella puedan sustraerla.
**Capas de la defensa en profundidad**
![image](https://user-images.githubusercontent.com/74509297/127354418-d36a0b22-4b99-467e-87f9-256f5b4ece7b.png)
 - **Seguridad física:** es la primera línea de defensa para proteger el hardware informático del centro de datos. La protección física del acceso a los edificios y el control del acceso al hardware de proceso del centro de datos son la primera línea de defensa.
 - **Identidad y acceso:** controla el acceso a la infraestructura y al control de cambios. En esta capa, es importante que realice lo siguiente:
   - Controle el acceso a la infraestructura y al control de cambios.
   - Use el inicio de sesión único (SSO)y la autenticación multifactor.
   - Audite los eventos y los cambios.
 - **Capa Perimetral:**  usa protección frente a ataques de denegación de servicio distribuido (DDoS) para filtrar los ataques a gran escala antes de que puedan causar una denegación de servicio para los usuarios. En esta capa, es importante que realice lo siguiente:
   - Use protección contra DDoS para filtrar los ataques a gran escala antes de que puedan afectar a la disponibilidad de un sistema para los usuarios.
   - Use firewalls perimetrales para identificar los ataques malintencionados contra la red y alertar sobre ellos.
 - **Capa de red:** limita la comunicación entre los recursos a través de controles de acceso y segmentación. En esta capa, es importante que realice lo siguiente:
   - Limite la comunicación entre los recursos.
   - Deniegue de forma predeterminada.
   - Restrinja el acceso entrante de Internet y limite el saliente cuando sea apropiado.
   - Implemente conectividad segura a las redes locales.
 - **Capa de proceso:** protege el acceso a las máquinas virtuales. En esta capa, es importante que realice lo siguiente:
   - Proteja el acceso a las máquinas virtuales.
   - Implemente la protección del punto de conexión de los dispositivos y mantenga los sistemas revisados y actualizados.
 - **Capa de aplicación:** ayuda a garantizar que las aplicaciones sean segurdas y estén libres de vulnerabilidades de seguridad.En esta capa, es importante que realice lo siguiente:
   - Garantice que las aplicaciones son seguras y están libres de vulnerabilidades.
   - Almacene los secretos de aplicación confidenciales en un medio de almacenamiento seguro.
   - Convierta la seguridad en un requisito de diseño en todo el desarrollo de aplicaciones.
 - **Capa de datos:** controla el acceso a los datos empresariales y de clientes que es necesario proteger. En casi todos los casos, los atacantes intentan conseguir datos:
   - Almacenados en una base de datos.
   - Almacenados en discos en máquinas virtuales.
   - Almacenados en aplicaciones de software como servicio (SaaS), como Office 365.
   - Administrados mediante el almacenamiento en la nube.
 
### Posición de seguridad
El nivel de seguridad es la capacidad de su organización de protegerse frente a amenazas de seguridad y responder a ellas
 - **Confidencialidad:** el principio de privilegios mínimos implica restringir el acceso a la información únicamente a los usuarios a las que se concede acceso de forma explícita, solo al nivel necesario para realizar su trabajo.
 - **Integridad:** Evitar cambios no autorizados en la información:
   - En reposo: cuando se almacenan.
   - En tránsito: cuando se transfieren de un lugar a otro, incluido desde un equipo local a la nube.
 - **Disponibilidad:** Asegúrese de que los servicios funcionan y que solo pueden acceder a ellos los usuarios autorizados.
 
### Azure Firewall
Es un servicio de seguridad de red administrado y basado en la nube que ayuda a proteger los recursos en las redes virtuales de Azure.
![image](https://user-images.githubusercontent.com/74509297/127358650-0e759a75-06bb-4846-9f8f-8c230a001ba4.png)

Azure Firewall proporciona muchas características, entre las que se incluyen:
 - Alta disponibilidad integrada
 - Escalabilidad en la nube sin restricciones.
 - Reglas de filtrado entrante y saliente.
 - Compatibilidad con la traducción de direcciones de red de destino (DNAT).
 - El registro de Azure Monitor.

Con Azure Firewall puede configurar:
 - Reglas de aplicación que definen los nombres de dominio completos (FQDN) a los que se puede acceder desde una subred.
 - Reglas de red que definen la dirección de origen, el protocolo, el puerto de destino y la dirección de destino.
 - Reglas de traducción de direcciones de red (NAT) que definen los puertos y las direcciones IP de destino para traducir las solicitudes entrantes.


## Módulo #16: Acceso seguro a las aplicaciones con servicios de identidad de Azure
**Autenticación:** es el proceso de establecimiento de la identidad de una persona o servicio que quiere acceder a un recurso. 
**Autorización:** es el proceso de establecer el nivel de acceso que tiene una persona o un servicio auttenticados.
![image](https://user-images.githubusercontent.com/74509297/127361634-c8e31287-e36a-4461-8dfe-46b7fde0788d.png)

### Azure Active Directory
Azure AD proporciona servicios como:
 - **Autenticación:** esto incluye la comprobación de la identidad para acceder a aplicaciones y recursos. También incluye funciones como el autoservicio de restablecimiento de contraseña, la autenticación multifactor, una lista personalizada de contraseñas prohibidas y servicios de bloqueo inteligente.
 - **Inicio de sesión único:** Gracias al SSO, los usuarios tienen que recordar un solo identificador y una sola contraseña para acceder a varias aplicaciones. Una sola identidad está asociada a un usuario, lo que simplifica el modelo de seguridad.
 - **Administración de aplicaciones:** Con Azure AD, puede administrar las aplicaciones en la nube y locales. 
 - **Administración de dispositivos:** Además de cuentas de usuarios individuales, Azure AD admite el registro de dispositivos. 









## Módulo #17: Creación de una estrategia de gobernanza en la nube en Azure
## Módulo #18: Examine los estándares de privacidad, cumplimiento y protección de datos en Azure
## Módulo #19: Planeación y administración de los costos de Azure
## Módulo #20: Elección de los servicios de Azure adecuados según los acuerdos de nivel de servicio y el ciclo de vida del servicio

Examen
Azure Monitor
Autentificación multifactor: algo que tienes, algo que sabes, algo que eres
Inovacion, cuando creas algo en la nube
Migración: mover algo hecho a la nube.
Azure government es solo para instancias de gobierno de EUA
