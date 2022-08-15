# Ánalisis y BBDD

En Microsoft Azure ofrece soluciones estructuradas y No-Estructuradas.

## Azure Cosmos DB

Es un servicio de BBDD NoSQL elástico e independiente al rendimiento y almacenamiento de las regiones. Este almacena los datos en un formato de secuencia de registro de átomos (ARS - Atom Registry Secuence), donde los datos se abstraen y se proyectan como una API.

También es compatible entre diferentes motores de BBDD:

* SQL
* Gremlin
* Cassandra
* mongoDB

## Azure SQL Database

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

## Azure SQL Managed Instance

Tiene muchas similitudes con Azure SQL Database, pero tiene algunas diferencias como:

* Comandos especificos para copias de seguridad
* Common Language Runtime (CLR). Entorno de ejecu
* Transacciones entre BBDD
* **NO** cuenta con escalado automático.

Con el servicio de **Azure Database Migration Service** nos permite migrar nuestras BBDD locales a la nube facilmente.

## Servicios para motores de BBDD específicos

Estos son los siguientes:

* Azure Database for MySQL
  * Ofrece alta disponibilidad, escalado en segundos y copias de seguridad automáticas.
* Azure Database for PostrgeSQL
  * Opción de servidor único.
    * Básico
    * Uso general
    * Optimizado
  * Hiperscala (Citus) para cargas de 100 GB o más

## Servicios de análisis de datos y Big Data

### Azure Synapse Analytics

Este servicio es usado para el análisis de datos de todo tipo: Sin procesar, refinados, seleccionados. Dicha inforamción puede venir por medi de recursos sin servidor o provisionados.

Este servicio es compatible con SQL y Apache Sparck.

### Azure HDInsight

Utiliza herramientas OpenSource para el análisis de datos, pudiendo procesar grandes volumenes de estos. Este puede crear clusteres de información de tipo Spark, Hadoop, Kafka, HBase, etc.... También admite ETLs.

### Azure Databrick

Descubre información de volúmenes masivos de datos.

Este es compatible con Apache Spark y funciona con Python, Scala, R, Java, SQL, TensorFlow, PyTorch Y Scikit-Learn.

### Azure Data Lake Analytics

Realiza un análisis de información bajo demanda, está enfocado a ETL en lugar de configurar el propio hardware, donde tiene un modelo Pay as you go.
