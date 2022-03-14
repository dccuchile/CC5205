# Sugerencia de datasets para el proyecto

* El dataset debe permitirles desarrollar un proceso de Minería de Datos donde se planteen **preguntas**, apliquen métodos descriptivos, predictivos, interpreten los resultados, etc.

* Lo ideal es que sea un volumen grande (muchas filas) y de alta dimensionalidad (varias decenas de columnas). 

* Si es un dataset de una competencia nos gustaría que planteen otras tareas alternativas con los datos y no sólo lo que se propone en la competencia. Un objetivo del proyecto es que ustedes puedan extraer conocimiento de los datos y no sólo maximizar "a ciegas" una tasa de aciertos. En caso de datasets con análisis públicos (como notebooks) demás está decir que su trabajo debe ser diferente.

* Una parte importante del proyecto y de manera general en la Minería de Datos es la reproducibilidad. En ese sentido en sus informes, reportes y presentaciones deben incluir referencias al dataset utilizado (links) siempre que sea posible.

### **Algunas ideas**

- **Awesome Data Chile**: Lista curada de fuentes de datos públicas sobre Chile recopilada por el IMFD: https://github.com/imfd/awesome-data-chile

- **COVID 19**: Hay varios datasets públicos respecto a la pandemia.
  - [Datos COVID19 Chile - Repositorio de Jorge Pérez](https://github.com/jorgeperezrojas/covid19-data)
  - [COVID19 Global Forecasting](https://www.kaggle.com/c/covid19-global-forecasting-week-1/overview)
  - [COVID-19 Open Research Dataset](https://www.semanticscholar.org/cord19)

- **Fairness & Bias (Data Science for Social Good)**: Un nuevo problema surge con el uso de Machine Learning y Data Mining en contextos sociales, como lo es el sesgo y la discriminación. Esto sugiere encontrar formas de crear modelos que permitan tratar a distintos grupos de manera "justa", pero la definición de justicia es compleja y los problemas se arrastran desde la generación de los datos, la interpretación de éstos y de los modelos, y de cómo repercuten en el futuro. Por ejemplo, un caso emblemático en Estados Unidos fue el de una empresa que ofrecía una predicción de riesgo de criminales por reincidir, y este puntaje es usado por jueces para ajustar las penas. Se observó que este puntaje era asignado de forma desequilibrada a distintos grupos raciales o étnicos. El objetivo de este proyecto es identificar estos sesgos y encontrar formas de disminuirlos, o concluir que no existe tal solución.

- - Lectura: [Machine Bias](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)
  - Análisis de los datos: https://www.propublica.org/article/how-we-analyzed-the-compas-recidivism-algorithm
  - Github: https://github.com/propublica/compas-analysis
  - Análisis y datos: https://github.com/caitlinkuhlman/bpdmtutorial/blob/master/tutorial.ipynb

- **Proceso Constituyente Chileno**: El portal de datos del Gobierno de Chile liberó la información de las Actas de Encuentros Locales Autoconvocados del Proceso Constituyente Chileno del 2016. La información se encuentra pública y ya se ha realizado trabajos para automatizar algunas tareas de clasificación de los datos.

- - Datos: https://github.com/uchile-nlp/ArgumentMining2017.
  - Paper: https://argmining2017.files.wordpress.com/2017/08/argmining2017-01.pdf

- **Caracterizar y clasificar problemas de Programación Competitiva**: Sitios como [http://codeforces.com](http://codeforces.com/), [http://www.spoj.com](http://www.spoj.com/), [http://a2oj.com](http://a2oj.com/), o [http://uhunt.felix-halim.net](http://uhunt.felix-halim.net/), entre otros, son repositorios de problemas de programación para competencias como la ACM-ICPC, la IEEExtreme, Google Code Jam, etc. Una aplicación interesante consiste en caracterizar los problemas, dadas las categorías (muchos de ellos están etiquetados con tags, o con los comentarios de los usuarios), clasificar un problema en sus categorías, o crear un "recomendador" de problemas de cierta dificultad y/o tema. Existen muchas clasificaciones de problemas, ya sea en los jueces online (como los referenciados anteriormente), o por usuarios que resuelven estos problemas (en blogs, github, etc.).

- - Ver también: [https://blog.anudeep2011.com/machine-learning-everywhere-why-not-in-competitive-programming](https://blog.anudeep2011.com/machine-learning-everywhere-why-not-in-competitive-programming/)

- **Tweets relacionados a crisis y desastres**: CrisisNLP es un recurso en el cual investigadores han compartido sus dataset relacionados a situaciones de emergencia, utilizados en sus investigaciones. https://crisisnlp.qcri.org/ 

- **Datos Cambio climáticos Minesterio de Ciencias**: Datos climatológicos recopilados por el minesterio de ciencias. https://github.com/MinCiencia/Datos-CambioClimatico

- **Datos climáticos**: mediciones históricas de Chile respecto a precipitaciones y temperaturas medias y máximas. Buscar en la pestaña de Observaciones. http://www.cr2.cl/ 

- **Caracterizar rendimiento estudiantil en Chile**: promedios de notas anuales de todos los alumnos de Chile con sus respectivos establecimientos desde 2002 hasta 2018. Descargar de http://datos.mineduc.cl/dashboards/19881/informacion-de-rendimiento-academico/ y descripcion de datos en http://datos.mineduc.cl/datasets/175906-er-rendimiento-por-alumno.download/

- **Analizar interacciones de Github en el tiempo**: interacciones varían desde commits hasta comentarios en issues y forks. https://www.gharchive.org/

- **Caracterizar series de anime**: explorar variaciones en el tiempo sobre tópicos de moda, estudios emergentes y gustos de usuarios. Contrastar éxito de series con las personas que trabajaron en esta. Datos generales pueden obtenerlos de https://www.kaggle.com/azathoth42/myanimelist (actualizado a mayo 2018), datos de equipos de producción preguntar a Juan-Pablo (actualizado a septiembre 2017).

-  **Datos publicados en Twitter durante el Estallido Social en Chile dl 2019**: caracterizar mensajes altamente polarizados para entender diferencias o similitudes existentes en la red de interacciones así como en el contenido de estos. Fuente: https://github.com/hsarmiento/chilean_unrest_dataset

#### **Otros temas sugeridos**
- Dataset de reviews de Amazon: https://www.kaggle.com/bittlingmayer/amazonreviews
- Dataset de reviews de cervezas: https://www.kaggle.com/rdoume/beerreviews (con texto: http://jmcauley.ucsd.edu/cse255/data/beer/)

#### **Más temas sugeridos (pedir al cuerpo docente)**

- Tweets de Ataques Terroristas de Manchester y Westminster, ambos ocurridos el 2017.
- Tweets de Chile geo-etiquetados del 2012 al 2017.


#### **Otros datasets disponibles**

- Buena fuente de datasets (recomendado): https://www.kaggle.com/datasets
- Otra buena fuente de datasets: https://blog.bigml.com/list-of-public-data-sources-fit-for-machine-learning/
- Zenodo: un repositorio open-access de datos y software científico: https://zenodo.org/ 
- Para preguntar si alguien tiene datos de X tema: https://www.reddit.com/r/datasets/

Chile:
- Microdatos del Censo Nacional de Población y Vivienda 2017. [http://www.censo2017.cl/microdatos/](http://www.censo2017.cl/microdatos/)
- Portal de Datos Abiertos. [http://datos.gob.cl](http://datos.gob.cl/)
- Gobierno Transparente. [http://transparenciaactiva.presidencia.cl](http://transparenciaactiva.presidencia.cl/)
- Transparencia Universidad de Chile. http://www.uchile.cl/transparencia
- Departamento de estadisticas e informacion de salud (SEIS): http://www.deis.cl/descargar-bases-de-datos-2/

APIs:
- Facebook API. [https://developers.facebook.com](https://developers.facebook.com/)
- Twitter API. [https://dev.twitter.com](https://dev.twitter.com/)

Otros:
- Wikipedia Data Dump. https://en.wikipedia.org/wiki/Wikipedia:Database_download
- Data.gov. [http://www.data.gov](http://www.data.gov/)
- Vox Articles published before March 2017. https://data.world/elenadata/vox-articles
- Stanford Network Analysis Project. [https://snap.stanford.edu](https://snap.stanford.edu/)
- Google BigQuery Public Datasets https://cloud.google.com/bigquery/public-data/
- Listado de datasets recopilado por KDnuggets. http://www.kdnuggets.com/datasets/index.html
- Listado de datasets recopilado por usuarios de Quora. https://www.quora.com/Where-can-I-find-large-datasets-open-to-the-public
- Datos de elementos y cosas que afectan la salud humana: https://healthdata.gov/search/type/dataset

Pidiendo acceso:
- Datos de cáncer en USA (necesitan pedir acceso): https://seer.cancer.gov/data/access.html
- Datasets varios (necesitan pedir acceso): https://bigml.com/gallery/datasets
- Datos de Yelp (necesitan pedir acceso): https://www.yelp.com/dataset
