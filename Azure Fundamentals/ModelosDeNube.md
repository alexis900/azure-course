# Modelos de servicios y tipo de nube

## On-Promise (Local)

Somos responsables del 100% de los servicios.

* Equipos
* Adecuación
* Mantenimiento
* Configuración
* Actualización
* ...

## Infraestructure as a Service (IaaS)

Solamente nos encargamos de la parte virtual de esa infraestructura, no de los equipos.

Nos tenemos que encargar del SO, actualizaciones, entorno de trabajo, etc...

* Ventajas
  * No tenemos CapEx, pagamos por lo que consumimos
  * Ágil
  * Administración compartida, la infraestructura la administra Azure
* Desventajas
  * Complicado al inicio según el grado de detalle que se requiere en aspectos de conociminto y tiempo.

## Platform as a Service (PaaS)

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

## Software as a Service (SaaS)

El proveedor administra el 100% del entorno y los usuarios solo utilizan la aplicación que se ejecuta en la nube. Por ejemplo Office Online, Outlook, CRM, ERP, etc...

* Desventajas
  * Se necesita una conexión a Internet.
  * Muy poco control.
  * Desempeño muy limitado.

## Serverless (Computo sin servidores)

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
  