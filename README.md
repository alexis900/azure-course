# Azure Fundamentals

## Ventajas y características

### ¿Qué es la nube?

La nube son instalaciones, que de forma independiente tienen electricidad, refrigeración y seguridad, son llamados Datacenters. Dentro de estos Datacenters se encuentran muchisimos computadores interconectados que podemos acceder a través de Internet para consumir servicios oficrecidos en la Nube.

Estos centros de datos están distibuidos a lo largo del mundo, donde este es el que tiene más.

Azure (Microsoft) intenta buscar que sus DataCenters sean 100% sustentables con energias limpias e incluso sumergirlos en el oceano para ahorrarse costos de refrigeración.

### ¿Para qué o Por qué?

* Computo
* Servidores
* Almacenamiento y BBDD
* Redes
* Inteligencia Artificial
* Desarrollo de software y más

`Todo lo que puedes hacer en una computadora se puede hacer en la nube pero más: **barato**, **ágil** y **seguro**.`

### Modelo de consumo

#### Pago por servicios usados

* Reduce costos operativos.

* Optimiza infraestructuras

* Escala según la necesidades

#### CapEx vs OpEx

* Gastos de capital (CapEx): Es la inversión de una infraestructura física, deducible a largo plazo.

* Gastos operativos (OpEx): Es la inversión en servicios o productos facturados al momento. No están fisicamente en tu empresa o proyecto.

### Ventajas

#### Confiablidiad y Alta Disponibilidad

Experiencia de usuario sin tiempo de inactividad perceptible, aunqué haya errores.

#### Escalabilidad

* Vertical: Aumentando de RAM/CPU a una VM. (En un solo equipo)
* Horizontal: Aumentando las instancias de recursos. (Si necesitamos más procesamiento, puede no ser solo en esa computadora, se pueden aumentar las VMs del procesamiento).

#### Elasticidad

Las aplicaciones siempre tendrás los recursos necesarios.

#### Agilidad

Instancia los recursos en la nube es muy rápido de implementar y configurar

#### Distribución geográfica

DataCenters de todo el mundo ofrecen el mejor rendimiento a cada región.

#### Recuperación ante desastres

Los datos se protegen con copias de seguridad, replicación y distribución geográfica.

## Modelos de servicios y tipo de nube

### On-Promise (Local)

Somos responsables del 100% de los servicios.

* Equipos
* Adecuación
* Mantenimiento
* Configuración
* Actualización
* ...

### Infraestructure as a Service (IaaS)

Solamente nos encargamos de la parte virtual de esa infraestructura, no de los equipos.

Nos tenemos que encargar del SO, actualizaciones, entorno de trabajo, etc...

* Ventajas
  * No tenemos CapEx, pagamos por lo que consumimos
  * Ágil
  * Administración compartida, la infraestructura la administra Azure
* Desventajas
  * Complicado al inicio según el grado de detalle que se requiere en aspectos de conociminto y tiempo.

### Platform as a Service (PaaS)

Se delegan más elementos al proveedor. Solamente nos debemos de preocupar del almacenamiento de datos y de las aplicaciones que vamos a desarrollar.

* Ventajas
El entoron (VMs, red, infraestructura) es administrador por el proveedor).
  * Solo te preocupas por el desarrollo.
  * Configuración mucho más ágil que IaaS
  * Enfocado al despliegue de las aplicaciones
* Desventajas
  * Puede ser más caro que IaaS, porqué te están dando las cosas más preparadas.
  * Problemas de compatibilidad según lo que se quiera hacer.
  * Dependencias con el proveedor.
  * Riesgos de seguridad
  * Limitante de idiomas, interfaz o recursos.

### Software as a Service (SaaS)

El proveedor administra el 100% del entorno y los usuarios solo utilizan la aplicación que se ejecuta en la nube. Por ejemplo Office Online, Outlook, CRM, ERP, etc...

* Desventajas
  * Se necesita una conexión a Internet.
  * Muy poco control.
  * Desempeño muy limitado.

### Serverless (Computo sin servidores)

Serverless **sí** usa servidores, aunqué el proveedor se encarga de todo ( aprovisiona, escala y administra toda la infraestructura). Esto sirve para ejecuta funciones o fracciones de código dirigidos por eventos.

* Ventajas
  * Altamente escalable
  * Está enfocada a la lógica de negocio (Por Ej.: Se dispara una alerta, realiza una acción especifica).
  * Ahorra mucho tiempo.
  * Pago por uso. (Por Ej. En las funciones, se puede pagar por función o evento ejecutado).

* Desventajas
  * No está diseñado para procesos extensos.
  * Detalles de desempeño.
  * Retos de testing y debugging.

## Tipos de nube

### Nube pública

La nube pública es accesible para todo el mundo. Este tipo de nube es propiedad de un proveedor. En este caso la nube pública, tal y como dice su nombre, se distribuye a través de Internet. Podemos conectarnos a los mismos recursos entre muchos usuarios.

### Nube privada

La nube privada solamente es accesible para algunos miembros de la organización.

Esta puede ser On-Premise o alojada en un centro de datos.

Una de sus desventajas es el costo.

### Nube híbrida

La nube híbrida es una combinación entre la nube pública y privada. Puede estar también combinado con funciones On-Premise.

## ¿Qué es Azure y como funciona?

### ¿Que és?

Azure es un proveedor de servicios en la nube que cuenta con más de 100 servicios a través de Internet.

* Ventajas
  * Está preparado para el futuro. (Está construyendo DataCenter alrededor del mundo).
  * Listo para crear a tu propio ritmo.
  * Listo para cualquier tipo de nube.
  * Confiable.

### ¿Como funciona?

Azure funciona a través de la virtualización, donde se puede realizar de forma local o en la nube de un DataCenter.

La virtualización es una abstracción de los elementos de un computador recibidos por un Hypervisor.

Los servidores están controlados por los **Fabric Controllers** que reciben instrucciones a través de un **Orquestador** y el cual recibe instrucciones del API de Azure a través del Portal de Azure, Azure CLI o PowerShell.

#### Azure Portal

Es el sitio web al que podemos ingresar para comenzar a trabajar con Azure.

#### Azure Marketplace

Es un mercado donde podemos encontrar estas instancias de recursos creadas por terceros, además de las herramientas propias.

## Cuentas de Azure

Una cuenta de Azure está formada por:

### Recursos

Són instancias de los servicios disponiles:

* Máquinas virtuales
* Almacenamiento
* FaaS (Functions as a Service)
* BBDD

### Grupos de recursos

Es un contenedor lógico donde se implementan y administran recursos de Azure. Por Ej. Aplicaciones web.

Los recursos solo formarán parte de un grupo de recursos, pero los recursos de un grupo se pueden comunicar con los recursos de otro.

### Suscripciones

Es una agrupación de cuentas de usuario y recursos creadas por estas cuentas. Pueden tener límites o cuotas definidas.

### Grupo de administración

Administra el acceso, directivas y cumplimiento de las suscripciones. Las suscripciones heredan las condiciones de su grupo.

## Suscripciones y grupos de administración

Se necesita una una suscripción de Azure para usar sus servicios:

* Desarrollador: Pagas por los servicios a medida que los utilices.
* Prueba: Experimentar con los productos, en algunos de manera gratuita.
* Subscripción: A través de un partner d ecompras de servicios de Azure.
* Estudiante: A través de un e-mail autorizado (.edu).

### Limites

* Facturación: Es la forma de facturarse. Cada subscripción tiene su propia factura.
* Control de acceso: Cada subscripción tiene sus directivas de acceso.

### ¿Cuándo se necesitan más suscripciones?

* Separación de entornos de trabajo como desarrollo, pruebas, aislamiento de datos, entre otros.
* Estructura Organizacional: Esta puede estar limitada según el presupuesto, tiempo de uso, por equipos o acceso de recursos.
* Facturación: Para facilitar el seguimiento de costos según los entornos, como producción, desarrollo, pruebas, etc...
* Límites por suscripción: Pueden haber algunas limitaciones de hardware por suscripción, entonces es necesario crear nuevas.

### Grupos de administración

#### Consideraciones

Se pueden tener hasta 10.000 grupos de administración en un único directorio, donde el arbol del grupo, puede tener hasta seis niveles de profundidad.

Cada grupo de adminsitración solo puede admitir un solo elemento primario, pero pueden tener muchos de secundarios.

## Recursos y grupos de recursos

Un recurso es un elemento administrable en Azure.

### Grupo de recursos

Un grupo de recursos es una agrupación de recursos relacionados para una solución.

#### Características

* Todos los recursos deben estar en un grupo de recursos.
* Un recurso solo puede pertenecer a un grupo.
* Los recursos pueden moverse entre los diferentes grupos.
* No se pueden anidad, es decir, un grupo no puede pertenecer a otro.
* Facilita la administración y organización.

Cuando eliminas un grupo de recursos, también elemena los recursos que contiene.

#### Autorización

Los grupos de recursos utiliza un control basado en roles (RBAC, Role Based Access Control), permitiendo el acceso solo a lo necesario.

#### Azure Resource Manager

Esta es una herramienta que permite administrar los recursos de forma masiva y de forma muy rápida a través de plantillas.

* Ventajas
  * Las plantillas están en formato JSON
  * Administra los recursos y grupos de recursos
  * Tiene capacidad de reutilización
  * RBAC (Role Based Access Control)
  * Etiquetas
  * Facturación

## Regiones y zonas de disponibilidad

Una región es un área geográfica con por lo menos un DataCenter, donde algunos servicios son exclusivos de una región.
  
También pueden existir algunas regiones especiales, como puede ser para el uso de los goviernos de algunos paises u otros para poder operar en dicho pais.

Azure es el proveedor con más regiones globales y en constante expansión.

### Zonas de disponibilidad

Una zona de disponibilidad es que haya dos DataCenters en una misma ubicación, con su propia electricidad, seguridad y regrigeración. Esto permite redundancia de servicios y datos ante errores u otros desastres.

No todas las regiones no son compatibles con zonas de disponibilidad, a parte puede generar más costos.

Las opciones del servicios en estas zonas de disponibilidad:

* Zona
* Redundancia de zona

### Pares de regiones

Regiones con por lo menos 500 Km de distancia entre ambas para replicar los recursos en caso de interrupciones.

* Desastres naturales
* Incendios
* Disturvios civiles
* Ausencia de electricidad
* Daños en la red fisica
* Etc...

## Ánalisis y BBDD

En Microsoft Azure ofrece soluciones estructuradas y No-Estructuradas.

### Azure Cosmos DB

Es un servicio de BBDD NoSQL elástico e independiente al rendimiento y almacenamiento de las regiones. Este almacena los datos en un formato de secuencia de registro de átomos (ARS - Atom Registry Secuence), donde los datos se abstraen y se proyectan como una API.

También es compatible entre diferentes motores de BBDD:

* SQL
* Gremlin
* Cassandra
* mongoDB

### Azure SQL Database

Es un servicio de BBDD estructuradas, basado en SQL Server.

* Alto rendimiento
* Confiable
* Administrada
* Compatible con NoSQL

Este servicio funciona como PaaS controlando las funciones administrativas de una BBDD:

* Actualizaciones
* Revisiones
* Copias de seguridad
* Supervisión

### Azure SQL Managed Instance

Tiene muchas similitudes con Azure SQL Database, pero tiene algunas diferencias como:

* Comandos especificos para copias de seguridad
* Common Language Runtime (CLR). Entorno de ejecu
* Transacciones entre BBDD
* **NO** cuenta con escalado automático.

Con el servicio de **Azure Database Migration Service** nos permite migrar nuestras BBDD locales a la nube facilmente.

### Servicios para motores de BBDD específicos

Estos son los siguientes:

* Azure Database for MySQL
  * Ofrece alta disponibilidad, escalado en segundos y copias de seguridad automáticas.
* Azure Database for PostrgeSQL
  * Opción de servidor único.
    * Básico
    * Uso general
    * Optimizado
  * Hiperscala (Citus) para cargas de 100 GB o más

### Servicios de análisis de datos y Big Data

#### Azure Synapse Analytics

Este servicio es usado para el análisis de datos de todo tipo: Sin procesar, refinados, seleccionados. Dicha inforamción puede venir por medi de recursos sin servidor o provisionados.

Este servicio es compatible con SQL y Apache Sparck.

#### Azure HDInsight

Utiliza herramientas OpenSource para el análisis de datos, pudiendo procesar grandes volumenes de estos. Este puede crear clusteres de información de tipo Spark, Hadoop, Kafka, HBase, etc.... También admite ETLs.

#### Azure Databrick

Descubre información de volúmenes masivos de datos.

Este es compatible con Apache Spark y funciona con Python, Scala, R, Java, SQL, TensorFlow, PyTorch Y Scikit-Learn.

#### Azure Data Lake Analytics

Realiza un análisis de información bajo demanda, está enfocado a ETL en lugar de configurar el propio hardware, donde tiene un modelo Pay as you go.

## Servicios de cómputo en la nube

### Azure Virtual Machines

Este es un servicio IaaS, donde nos encargaremos de administrar de la parte virtual de la computadora. Nos permite hacer una migración de nuestras máquinas On-Premise a la nube.

#### Azure Batch

Es un conjunto de máquinas virtuales, donde podemos configurarlas en minutos para que sean idénticas, donde pueden aumentar o disminuir estas máquinas automáticamente con reglas.

### Azure Container Instances

Un contenedor es como una máquina virtual más liviana, donde solo estamos "virtualizando" el sistema operativa, e incluso sus funciones. Este no tiene acceso a memória RAM, procesamiento, almacenamiento...
Estos contenedores estás aislados.

Este servicio de Azure Container Instances, es un PaaS para la ejecución de estos.

#### Azure Kubernetes Service

Este servicio permite orquestar (automátización y administración) de contenedores en volumen.

### Azure Functions

Nos permite tener funciones o porciones de código que van a respoder a eventos. Por Ej. Peticiones REST, temporizadores, etc...

Estas funciones escalan automáticamente según el uso de estas.

#### Azure Logic Apps

Es un servicio de flujos de trabajo basado en eventos, donde cuenta una GUI para hacerlo de forma visual o en formato JSON. Podemos tener más de 200 conectores y bloques.

### Windows Virtual Desktop

Este servicio permite tener Windows en cualquier sitio.

Tenemos una comptatibilidad con cualquier equipo, aumenta la seguridad (hay un ambiente aislado con el equipo). Se pueden utilizar licencias propias.

## Almacenamiento

Azure nos provee la posibilidad de utilizar HDDs, SSD e incluso algunos de calidad premium que podremos usar para cuestiones especificas.

### Azure Blob (Binary Large Object) Storage

Este servicio lo usaremos principalmente para un almacenamiento no estructurado, que no tenga ningún tipo de restricción y además puede soportar miles de cargas simultáneas. Este es ideal para guardar audio, video e imágen.

También es excelente para hacer respaldos, al no ser estructurado lo podremos guardar ahí mismo.

Por otro lado, cuenta con una opción de análisis de datos conveniente si por ejemplo una máquina virtual tiene más de 8 TB de información.

#### Niveles de acceso

* Frecuente: Imágenes o descargas de un sitio web. Són más rápidos de consultar y acceder a ellos.
* Esporádico (30 días): Reportes mensuales, facturas, etc...
* Archivo (180 días): Copias de seguridad. Se tarda más en acceder a estos datos.

Es importante saber esto porqué cuando hacemos esto consulta a estos datos van a haber dos factores involucrados:

* Velocidad de acceso
* Costo de la transacción o de consulta

### Azure Files

Nos permite almacenar archivos, donde consiste en compartir recursos administrados en la nube bajo los protocolos SMB o NFS, pudiendo estar tanto en local como en la nube.

Se vuelve muy útil si muchos recursos de Azure, con distintas aplicaciones, personas, máquinas virtuales quieren acceder a estos archivos.

## Servicios de red

Los servicios de red en Azure, no nos tenemos que preocupar del cableado estructurado, solamentente nos tenemos que preocupar de las redes virtuales para configurarlas, hacer sus conexiones y garantizar su seguridad.

### Azure Virtual Network

Este permite a los recursos de Azure comunicarse entre sí, con los usuarios de Internet y equipos On-Promise. Este también permite aislar y segregar los recursos por grupos de red.

Como nos estamos comunicando con Internet, deberemos de usar redes virtuales o puntos de conexión de servicio.

#### Enrutamiento de la red

Podemos enrutar el tráfico de esta red a través de Tablas de ruta o con el protocolo de Puerta de enlace de Borde (BGP).

#### Filtrado del tráfico de la red

Podemos considerar el filtrado del trafico de la red. Esto lo podemos generar a través de los grupos de seguridad de red o aplicaciones de red.

### Azure VPN Gateway

Este servicio conecta las redes locales de Azure a través de una VPN de sitio/sitio o de sitio/punto a través de protocolos IPsec e IKE.

La comunicación con recursos locales también pueden ser con redes virtuales pueden configurarse de Point-tosite (P2S) o Virtual Private Networks (VPN), donde nos permite crear una conexión segura a la red virtual (☁️) desde un cliente individual (desde Internet).

Virtual Private Network (VPN) Site-to-Site permiten vincular la red del centro de datos local (On-Promises) con la red de Azure, creando un efecto que todos los equipos están en la misma red.

### Azure ExpressRoute

Este provee una conexión dedicada a la nube de Azure.

## Inteligencia Artifical

La Inteligencia Artificial (AI) tiene dos enfoques básicos de ese razonamiento que busca asemejarse a las personas:

* Deep learning: Utiliza redes neuronales para descubrir, aprender y crecer. Va a tomar información, la analizará y buscará aprender con esta.
* Machine learning: Utiliza datos existentes para entrenar modelos y pronosticar. Intenta predecir el futuro con provabilidades.

### Azure Machine Learning

Este servicio como Paas nos sirve para poder realizar preducciones conectandonos a datos para entrenar y probar modelos. Este nos ofrece el control total del diseño y entrenamiento de dichos algoritmos y modelos de entrenamiento.

### Azure Cognitive Services

Este servicio proporciona a la computadora la capacidad de tener sentidos a través de la IA. A la IA le pueden llegar a permitir oír, hablar, entender y pensar. Este tipo de servicios no requiere conocimientos de Machine Learning ni Data Science a través de APIs.

Tenemos diferentes categorias:

* Lenguaje: Traducir en voz, comandos.
* Voz: Conversión de voz a texto
* Visión: Reconocimiento de imágenes.
* Decisión: Tomar decisiones basada en la información dada.


### Azure Bot Service

Nos permite crear bots o agentes virtuales, tiene su propio framework para poder desarrollar con código. Se puede usar en Servicios de Atención al Cliente, etc...

## Azure DevOps Services

### Azure Repos

Nos permite crear repositorios de código fuente centralizado para publicar código y colaborar. Estos repositorios están albergados en esta plataforma y también están centralizados para el uso de la organización.

### Azure Board

Nos permite crear tableros para la gestión de proyectos como Kanban, informes, incidencias, epics, etc...

### Azure Pipelines

Nos ayuda a automátizar los Continuos Integration (CI) y Continuos Delivery (CD).

### Azure Artifacts

Nos permite crear repositorios para alojar artefactos que se incluyen en el flujo de pruebas o implementación. Este servicio puede estar acompañado de Azure Pipelines.

### Azure Test Plans

Són herramientas de prubeas automatizadas para garantizar la calidad antes de lanzar el software.

### GitHub Actions

Nos permite automatizar los flujos de trabajo basados en triggers, especialmente para CI/CD. Este servicio se puede conectar con Azure muy facilmente.

### Azure DevTest Labs

Automatizar pruebas o espacios de pruebas en el proceso de compilación, configuración y anulación de VMs cuando no se usen.

## Monitoreo y supervisión

### Azure Advisor

Este servicio nos permite evaluar los recursos y brindar recomendaciones y notificaciones para mejorar a través o su API. Podemos llegar a configuralo para que nos envie SMSs o e-mails.

### Azure Monitor

Este servicio nos permite recopilar, analizar y mostrar los datos para tomar acciones basadas en métricas del entorno.

### Azure Service Health

Este servicio nos da una vista personalizada del estado de los servicios, regiones y recursos de Azure.

## Administración y configuración de entorno

Al trabajar en la nube es necesario tener un buen control y administración del trabajo. Azure nos da las herramientas para la administración de trabajo, las cuales pueden ser visuales o básada en linea de comandos.

### Azure Portal

Es una consola unificada basada en la web que proporciona una alternativa a las herramientas por línea de comandos. Con esta, se pueden administrar su subscripción de Azure medieante una GUI.

### Azure Mobile App

Una aplicación móvil para administrar información de interés de nuestros servicios contratados.

### Herramientas CLI

* Azure PowerShell
* Azure CLI
* Cloud Shell

### Azure Resources Manager Templates

Es un administrador de plantillas de recursos.

Estas plantillas usan el formato JSON, donde comprueba el estado antes de ejecutarse. Este define el estado y la configuración de cada recurso, la plantilla hace el resto.

## Serverless

Contrario a lo que pareciera indicar el nombre, si se usan servidores. Se realiza una abstracción de todo lo que se refiere al servidor, es decir, no se tiene contacto total al los servidores físicos de Azure, pero si com los servicios que estos nos ofrecen.

### Azure Functions

Este servicio se encarga de almacenar métodos o funciones. Pedazos de código que se van a ejecutar cuando se cumpla un evento basado en disparadores o triggers. Este es compatible con algunos lenguajes de programación como C#, JS, Python, TypeScript, Java, Shell.

Este servicio se cobrará a razón del número de ejecuciones sobre el tiempo.

### Azure Logic Apps

Ideal para automatizar y organizar de menra No-Code o Low-Code.

Este servicio se cobrará a razón del número de ejecuciones sobre el tiempo y el tipo de conectores.

## IoT

El Internet of Things (IoT), describe la red de objetos físicos (cosas), que llevan sensores integrados, software y otras tecnologías con el fin de conectar e intercanviar datos con otros dispositivos y sistemas a través de Internet.

Estos datos pueden venir de diferentes sensores, como de ubicación geográfica (GPS), sonido, movimiento, biométricos, etc...

### Azure IoT Hub

Este servicio es un centro de mensajes entre las aplicaciones IoT y dichos dispositivos. Se puede controlar remotamente manual o automáticamente, aunqué cuenta con supervisión.

### Azure IoT Central

Está basado en IoT Hub con interfaz visual, ya que esta otra está más enfocado a la aplicaión o desarrollo. Este también posee plantillas para escenarios comunes.

### Azure Sphere

Son dispositivos de hardware de la propia Azure, intenta solucionar la estandarización del hardware y software y conectandose a Azure en la nube. Estos dispositivos pueden llegar a utilizar cuando la seguridad es crítica, como un terminal de pagos.

## Servicios de seguridad

### Azure Security Center

Es un servicio que brida de visibilidad del nivel de seguridad de los servicios en Azure y en local, donde supervisa la configuración de seguridad y puede llegar automáticamente a aplicar cambios en relación a la seguridad. También da recomendaciones al servicio.

Puede detectar y bloquear amenazas de malware con ML detectando ataques e investigar dichas amenazas. También proporciona control de acceso cuando sea necesario.

En la medida del nivel de seguridad permite notificar el estado actual, mejorar el nivel y comparar puntos de referencia.

### Azure Sentinel

Este es un Administrador de Eventos y de la seguridad de la Información (SIEM) en la nube de análisis de seguridad y amenazas. También se investigan con IA y responder a los incidentes de forma proactiva.

### Azure Key Vault

Es un servicio centralizado para almacenar secretos o datos confidenciales en un solo lugar, como:

* Secretos
* Claves de cifrado
* Cetificados SSL/TLS
* Respaldos por módulos de seguridad de Hardware

### Azure Dedicated Host

Son servidores físicos que no se comparten con nadie más. Se trataría como nube privada.

Este proporciona visibilidad y control, asegurando los requisitos de cumplimiento. Este, al ser más personalizable, puede tener un mayor costo.

### Seguridad en red

* Azure Firewall: Permite enrutar o filtrar el tráfico.
* Azure DDoS Protection: Evita ataques DDoS.

Esto se puede llegar a combinar varios de estos servicios para aumentar la seguridad.

### Servicios de identidad

Tenemos diferntes tipos de autorizaciones:

* Auténtificación (AuthN): Solicita las credenciales legitimas.
* Autorización (AuthZ): Establece el nivel de acceso a una persona o servicio autenticado.

Para aplicar esto en Azure tenemos dos servicios:

* Azure Active Directory es un servicio que nos permite registrar esas suscripciones, grupos de administración, roles para tener la seguridad y con qué permisos se accede. Se puede usar en la nube o en On-Promise.
* Inicio de sesión único (SSO): Permite recordar un solo identificador y una sola contraseña para acceder a varias aplicaciones.

Una buena autenticación tiene por lo menos 3 elementos:

* Algo que sabes (usuario/contraseña)
* Algo que tienes (tarjeta de identificación)
* Algo que eres (datos biometricos)

#### Azure AD Multi-Factor Authentication

Este servicio proporciona funcionalidades de autenticación multifactor.

## Privacidad, cumplimiento y protección de datos

Los datos de nuestros clientes, **NO** son nuestros datos.

El cumplimiento es cumplir con una ley, estándar, conjunto de directrices, normas o requerimientos globales, gubernamentales, sectoriales, regionales.

### Declaración de privacidad

Explica qué datos personaler se recopilan, cómo los usa y para qué. Esta declaración de privacidad abarca a todos sus servicios, sitios, software, servidores y dispositivos.

### Terminos de los servicios en linea

Es un contrato legal entre Microsoft y el cliente, donde detalla las obligaciones de ambas partes al  procesamiento y seguridad de los datos. Esto aplica a servicios bajo una licencia.

### Anexo de protección de datos

Define estos términos de seguridad y procesamiento de datos para los servicios en línea cumplimentando de leyes, revelación de datos y la seguridad de los datos.

## Planeación y administración de costos

Azure nos proporciona una herramienta para poder proyectar estos costos.

### Calculadora de costo total de propiedad (TOC)

Esta calculadora nos permite calcular el costo de Azure vs. tener nuestros servicios en local, si tenemos pensado migrar a la nube.

## Acuerdos de nivel de servicio

La composición del acuerdo de nivel de servicio de los servicios de Azure que use le ayudará a conocer las garantías que puede esperar.

La disponibilidad de los servicios que usa afecta al tiempo de actividad de las aplicaciones que se compilan en Azure.

Cada acuerdo de nivel de servicio especifica el plazo en el que se debe enviar la reclamación y el plazo para que Microsoft lo procese. En muchos servicios, la reclamación debe enviarse antes de que finalice el mes natural.