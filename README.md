# **Practica-KC-BD-Architecture**
Este proyecto es parte del Módulo de Arquitectura Big Data, donde he trabajado con varias tecnologías de la arquitectura Hadoop y herramientas asociadas. A lo largo del modulo, he creado diversos clústeres en *Google Cloud Dataproc, diversas instancias virtuales de Google Compute Engine, Redes VPC, Cloud Storage y mas*.
---

*Tecnologías utilizadas:*</p>
_1- Google Cloud Dataproc:_ Utilizamos Google Cloud Dataproc para crear y gestionar un clúster Hadoop. Dataproc es una plataforma administrada que facilita el trabajo con frameworks como Hadoop y Spark , permitiéndonos ejecutar y gestionar grandes volúmenes de datos con eficiencia en la nube.

_2- Hadoop:_ Hadoop es la base de esta arquitectura, y se utiliza para distribuir el procesamiento de grandes volúmenes de datos. La configuración de HDFS (Hadoop Distributed File System) permite almacenar y gestionar los datos de manera distribuida en el clúster.

_3- Hive:_ Utilizamos Hive para realizar consultas SQL sobre los datos almacenados en Hadoop. Hive proporciona una interfaz similar a SQL para facilitar el análisis de grandes cantidades de datos. Esto nos permitió ejecutar consultas sobre los datos y realizar transformaciones de manera eficiente.

_4- Elasticsearch:_ Implementamos Elasticsearch para almacenar y buscar datos indexados. Elasticsearch es una base de datos distribuida de búsqueda que permite realizar búsquedas rápidas y complejas sobre grandes volúmenes de datos. Fue utilizado para almacenar registros de datos y permitir consultas más rápidas y efectivas.

_5- Kibana:_ Usamos Kibana como herramienta de visualización de datos para interactuar con Elasticsearch. Kibana se conecta a Elasticsearch para crear gráficos y paneles dinámicos que permiten una visualización clara y comprensible de los datos procesados ​​y almacenados.

---

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
A lo largo de esta práctica, he trabajado con *Google Cloud Dataproc, Hadoop, Hive, Elasticsearch y Kibana*, creando una infraestructura robusta y escalable para el procesamiento y análisis de grandes volúmenes de datos.
Este flujo de trabajo me ha proporcionado una comprensión más profunda de cómo las arquitecturas modernas de Big Data funcionan en la nube y cómo integran herramientas para maximizar la eficiencia y la facilidad de uso.
