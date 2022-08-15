# Almacenamiento

Azure nos provee la posibilidad de utilizar HDDs, SSD e incluso algunos de calidad premium que podremos usar para cuestiones especificas.

## Azure Blob (Binary Large Object) Storage

Este servicio lo usaremos principalmente para un almacenamiento no estructurado, que no tenga ningún tipo de restricción y además puede soportar miles de cargas simultáneas. Este es ideal para guardar audio, video e imágen.

También es excelente para hacer respaldos, al no ser estructurado lo podremos guardar ahí mismo.

Por otro lado, cuenta con una opción de análisis de datos conveniente si por ejemplo una máquina virtual tiene más de 8 TB de información.

### Niveles de acceso

* Frecuente: Imágenes o descargas de un sitio web. Són más rápidos de consultar y acceder a ellos.
* Esporádico (30 días): Reportes mensuales, facturas, etc...
* Archivo (180 días): Copias de seguridad. Se tarda más en acceder a estos datos.

Es importante saber esto porqué cuando hacemos esto consulta a estos datos van a haber dos factores involucrados:

* Velocidad de acceso
* Costo de la transacción o de consulta

## Azure Files

Nos permite almacenar archivos, donde consiste en compartir recursos administrados en la nube bajo los protocolos SMB o NFS, pudiendo estar tanto en local como en la nube.

Se vuelve muy útil si muchos recursos de Azure, con distintas aplicaciones, personas, máquinas virtuales quieren acceder a estos archivos.
