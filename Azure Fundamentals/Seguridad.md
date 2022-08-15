# Servicios de seguridad

## Azure Security Center

Es un servicio que brida de visibilidad del nivel de seguridad de los servicios en Azure y en local, donde supervisa la configuración de seguridad y puede llegar automáticamente a aplicar cambios en relación a la seguridad. También da recomendaciones al servicio.

Puede detectar y bloquear amenazas de malware con ML detectando ataques e investigar dichas amenazas. También proporciona control de acceso cuando sea necesario.

En la medida del nivel de seguridad permite notificar el estado actual, mejorar el nivel y comparar puntos de referencia.

## Azure Sentinel

Este es un Administrador de Eventos y de la seguridad de la Información (SIEM) en la nube de análisis de seguridad y amenazas. También se investigan con IA y responder a los incidentes de forma proactiva.

## Azure Key Vault

Es un servicio centralizado para almacenar secretos o datos confidenciales en un solo lugar, como:

* Secretos
* Claves de cifrado
* Cetificados SSL/TLS
* Respaldos por módulos de seguridad de Hardware

## Azure Dedicated Host

Son servidores físicos que no se comparten con nadie más. Se trataría como nube privada.

Este proporciona visibilidad y control, asegurando los requisitos de cumplimiento. Este, al ser más personalizable, puede tener un mayor costo.

## Seguridad en red

* Azure Firewall: Permite enrutar o filtrar el tráfico.
* Azure DDoS Protection: Evita ataques DDoS.

Esto se puede llegar a combinar varios de estos servicios para aumentar la seguridad.

## Servicios de identidad

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

### Azure AD Multi-Factor Authentication

Este servicio proporciona funcionalidades de autenticación multifactor.
