# Azure 🔷 PaaS

PaaS (Platform as a Service), permite desplegar nuestras aplicaciones y hacerlas disponibles al público con servicios de almacenamiento y BBDD.

## Grupo de recursos

Un grupo de recursos permite englobar un gran repositorio de todos los componentes de una solución.

## Almacenamiento

### Tipos de almacenamiento

El almacenamiento en Azure tiene que ver con cuatro matices y cada uno de estos tiene un objetivo diferente.

Lo primero que necesitamos es saber que esperamos con este almacenamiento.

#### File

Crea unidades de disco duro virtual. Esta se puede montar en muchas computadoras al mismo tiempo y en diferentes sistemas operativos.

#### Blob (Binary Large Object)

Es un diso duro virtual gigante, donde nos permite almacenar teras de información sin ningún problema.

Este se puede dividir entre el **frío**, con información que no se utiliza pero se quiere guardar (Por ej. Backups); y en **activo**, se busca información como vídeo o imágenes de manera constante.

#### Queue (Colas)

Van a pasar por partes las solicitudes para que sean atendidas una por una. Esto es útil para evitar cuellos de botella en tráfico de alta demanda.

#### Table

Es capaz de almacenar registros creando una especie de base de datos.

### Azure Storage Explorer

Azure Storage Explorer es una herramienta para poder acceder facilmente a nuestro grupo de almacenamiento.
