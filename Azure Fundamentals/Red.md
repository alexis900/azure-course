# Servicios de red

Los servicios de red en Azure, no nos tenemos que preocupar del cableado estructurado, solamentente nos tenemos que preocupar de las redes virtuales para configurarlas, hacer sus conexiones y garantizar su seguridad.

## Azure Virtual Network

Este permite a los recursos de Azure comunicarse entre sí, con los usuarios de Internet y equipos On-Promise. Este también permite aislar y segregar los recursos por grupos de red.

Como nos estamos comunicando con Internet, deberemos de usar redes virtuales o puntos de conexión de servicio.

### Enrutamiento de la red

Podemos enrutar el tráfico de esta red a través de Tablas de ruta o con el protocolo de Puerta de enlace de Borde (BGP).

### Filtrado del tráfico de la red

Podemos considerar el filtrado del trafico de la red. Esto lo podemos generar a través de los grupos de seguridad de red o aplicaciones de red.

## Azure VPN Gateway

Este servicio conecta las redes locales de Azure a través de una VPN de sitio/sitio o de sitio/punto a través de protocolos IPsec e IKE.

La comunicación con recursos locales también pueden ser con redes virtuales pueden configurarse de Point-tosite (P2S) o Virtual Private Networks (VPN), donde nos permite crear una conexión segura a la red virtual (☁️) desde un cliente individual (desde Internet).

Virtual Private Network (VPN) Site-to-Site permiten vincular la red del centro de datos local (On-Promises) con la red de Azure, creando un efecto que todos los equipos están en la misma red.

## Azure ExpressRoute

Este provee una conexión dedicada a la nube de Azure.
