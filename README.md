#  Practica-KC-BD-Arquitectura  

Este proyecto forma parte del **Módulo de Arquitectura Big Data**, donde trabajamos con diversas tecnologías del ecosistema **Hadoop** y herramientas asociadas. Implementamos clústeres en **Google Cloud Dataproc**, configuramos **instancias virtuales en Google Compute Engine**, utilizamos **Redes VPC, Cloud Storage** y más.

---

##📌  Tecnologías utilizadas  

### 1️ Google Cloud Dataproc  
Plataforma administrada para la creación y gestión de clústeres **Hadoop** y **Spark** en la nube, permitiendo el procesamiento eficiente de grandes volúmenes de datos.  

### 2️ Hadoop  
Framework base de la arquitectura utilizada. Se encargó de la distribución y procesamiento de datos a gran escala, gestionados a través de **HDFS (Hadoop Distributed File System)**.  

### 3️ Hive  
Herramienta que permite ejecutar **consultas SQL** sobre datos almacenados en Hadoop, facilitando el análisis y transformación de información mediante su interfaz similar a SQL.  

### 4️ Elasticsearch  
Base de datos distribuida optimizada para **búsquedas rápidas y complejas** sobre grandes volúmenes de datos. Se utilizó para almacenar registros de datos y mejorar la eficiencia en la consulta de información.  

### 5️ Kibana  
Herramienta de **visualización de datos**, conectada a Elasticsearch para la generación de gráficos, paneles interactivos y visualización clara de los datos procesados.  

---

## 📌 Pasos del Proyecto  

###  1. Creación del Clúster en Google Cloud Dataproc  
Se configuró un **clúster Dataproc** con nodos **maestros y trabajadores**, permitiendo la ejecución de herramientas como **Hadoop** y **Hive**.  

###  2. Configuración de Hive y Hadoop  
Nos conectamos al nodo maestro mediante **SSH** para configurar **Hive y Hadoop**, habilitando el almacenamiento distribuido y la ejecución de consultas SQL sobre los datos.  

###  3. Implementación de Elasticsearch  
Se instaló y configuró **Elasticsearch** en una **VM independiente**, habilitando la indexación y búsqueda eficiente de datos.  
Se definieron **reglas de firewall** en Google Cloud para permitir tráfico en los puertos:  
- **9200** (Elasticsearch)  
- **5601** (Kibana)  

###  4. Conexión entre Hadoop y Elasticsearch  
Se estableció la conexión entre el clúster **Hadoop** y **Elasticsearch**, permitiendo la carga y consulta eficiente de datos.  
Utilizamos **curl** para insertar documentos en Elasticsearch, asegurando la conectividad mediante reglas de red y configuraciones de firewall.  

###  5. Carga de datos en Elasticsearch  
Se usó la **API de Elasticsearch** para insertar documentos en el índice **alumnos** desde Hadoop, optimizando la carga masiva de información.  

###  6. Visualización de datos con Kibana  
Finalmente, se configuró **Kibana** para visualizar y explorar los datos almacenados en **Elasticsearch**, permitiendo la creación de gráficos y paneles interactivos.  

---

## 📌 Conclusión  

A lo largo de esta práctica, trabajamos con **Google Cloud Dataproc, Hadoop, Hive, Elasticsearch y Kibana**, construyendo una infraestructura robusta y escalable para el **procesamiento y análisis de datos** en la nube.  

Este proyecto brindó una comprensión más profunda sobre las **arquitecturas modernas de Big Data**, su integración con servicios en la nube y cómo optimizar el flujo de datos para mejorar la eficiencia y escalabilidad. 🚀  



---------------------------------------------------------------------------------------------------------------------------------------------------


# **Practica-KC-BD-Architecture**
Este proyecto es parte del Módulo de Arquitectura Big Data, donde he trabajado con varias tecnologías de la arquitectura Hadoop y herramientas asociadas. A lo largo del modulo, he creado diversos clústeres en Google Cloud Dataproc, diversas instancias virtuales de Google Compute Engine, Redes VPC, Cloud Storage y mas.

*Tecnologías utilizadas:*</p>
_1- Google Cloud Dataproc:_ Utilizamos Google Cloud Dataproc para crear y gestionar un clúster Hadoop. Dataproc es una plataforma administrada que facilita el trabajo con frameworks como Hadoop y Spark , permitiéndonos ejecutar y gestionar grandes volúmenes de datos con eficiencia en la nube.

_2- Hadoop:_ Hadoop es la base de esta arquitectura, y se utiliza para distribuir el procesamiento de grandes volúmenes de datos. La configuración de HDFS (Hadoop Distributed File System) permite almacenar y gestionar los datos de manera distribuida en el clúster.

_3- Hive:_ Utilizamos Hive para realizar consultas SQL sobre los datos almacenados en Hadoop. Hive proporciona una interfaz similar a SQL para facilitar el análisis de grandes cantidades de datos. Esto nos permitió ejecutar consultas sobre los datos y realizar transformaciones de manera eficiente.

_4- Elasticsearch:_ Implementamos Elasticsearch para almacenar y buscar datos indexados. Elasticsearch es una base de datos distribuida de búsqueda que permite realizar búsquedas rápidas y complejas sobre grandes volúmenes de datos. Fue utilizado para almacenar registros de datos y permitir consultas más rápidas y efectivas.

_5- Kibana:_ Usamos Kibana como herramienta de visualización de datos para interactuar con Elasticsearch. Kibana se conecta a Elasticsearch para crear gráficos y paneles dinámicos que permiten una visualización clara y comprensible de los datos procesados ​​y almacenados.

<b>*Pasos del Proyecto:*</b>
1. Creación del Clúster en Google Cloud Dataproc
Iniciamos creando un clúster Dataproc en Google Cloud.Este clúster incluye los nodos maestros y trabajadores necesarios para ejecutar aplicaciones Hadoop, como Hive y otros componentes de procesamiento de datos.

2. Configuración de Hive y Hadoop en el Clúster
Una vez creado el clúster, onectamos a través de SSH a la VM del nodo maestro y configuramos Hive y Hadoop. Con esto, habilitamos el procesamiento y almacenamiento de grandes volúmenes de datos, facilitando el análisis mediante consultas SQL.

3. Implementación de Elasticsearch
Luego, instalamos y configuramos Elasticsearch en una VM adicional para almacenar los datos procesados ​​y permitir búsquedas eficientes.Para ello, configuramos las reglas de firewall en Google Cloud para permitir el tráfico hacia el puerto 9200 de la VM que ejecuta Elasticsearch y 5601 que ejecuta Kibana.

4. Conexión entre Hadoop y Elasticsearch
Configuramos la conexión entre el clúster de Hadoop y Elasticsearch para poder cargar y procesar los datos de manera eficiente. Utilizamos curl para agregar documentos al índice de Elasticsearch y aseguramos que las conexiones entre las instancias fueran posibles mediante el ajuste de las configuraciones de red y las reglas de firewall.

5. Carga de datos en Elasticsearch
Usamos la herramienta API de Elasticsearch para cargar documentos de datos en el índice alumnos desde el clúster de Hadoop. Esto nos permitió insertar varios documentos a la vez de manera eficiente.

6. Visualización de datos con Kibana
Una vez que los datos fueron cargados y almacenados en Elasticsearch, configuramos Kibana para visualizar y explorar los datos de manera interactiva. Kibana se conecta a Elasticsearch y permite crear paneles y gráficos que visualizan los datos de manera clara.

_<p>.**Conclusión**.</p>_
A lo largo de esta práctica, he trabajado con Google Cloud Dataproc, Hadoop, Hive, Elasticsearch y Kibana, creando una infraestructura robusta y escalable para el procesamiento y análisis de grandes volúmenes de datos. Este flujo de trabajo me ha proporcionado una comprensión más profunda de cómo las arquitecturas modernas de Big Data funcionan en la nube y cómo integran herramientas para maximizar la eficiencia y la facilidad de uso.
