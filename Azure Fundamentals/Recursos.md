# Recursos y grupos de recursos

Un recurso es un elemento administrable en Azure.

## Grupo de recursos

Un grupo de recursos es una agrupación de recursos relacionados para una solución.

### Características

* Todos los recursos deben estar en un grupo de recursos.
* Un recurso solo puede pertenecer a un grupo.
* Los recursos pueden moverse entre los diferentes grupos.
* No se pueden anidad, es decir, un grupo no puede pertenecer a otro.
* Facilita la administración y organización.

Cuando eliminas un grupo de recursos, también elemena los recursos que contiene.

### Autorización

Los grupos de recursos utiliza un control basado en roles (RBAC, Role Based Access Control), permitiendo el acceso solo a lo necesario.

### Azure Resource Manager

Esta es una herramienta que permite administrar los recursos de forma masiva y de forma muy rápida a través de plantillas.

* Ventajas
  * Las plantillas están en formato JSON
  * Administra los recursos y grupos de recursos
  * Tiene capacidad de reutilización
  * RBAC (Role Based Access Control)
  * Etiquetas
  * Facturación
  