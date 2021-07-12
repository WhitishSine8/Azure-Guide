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
  - **Azure App Service:** sirve para compilar, implementar y escalar de forma rápida aplicaciones de API, móviles y web de nivel empresarial que puedan ejecutarse en cualquier plataforma. 
  - **Azure Functions:** es utilizada cuando la unica preocupación es el código que ejecuta el servicio y no la infraestructura o plataforma subyacente. 
 

 ## Módulo #5: Exploración de los servicios de red de Azure.
 ## Módulo #6: Exploración de los servicios de Azure Storage.
 ## Módulo #7: Exploración de los servicios de análisis y bases de datos de Azure.
