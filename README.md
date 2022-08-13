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
