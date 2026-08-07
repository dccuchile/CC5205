**Proyecto de Minería de Datos**

El proyecto del curso de Minería de Datos tiene como objetivo que los estudiantes trabajen en equipo siguiendo la metodología completa de minería de datos. Esto incluye la selección de un conjunto de datos, su exploración y limpieza, la formulación de preguntas que puedan ser respondidas mediante técnicas de aprendizaje automático, la aplicación de modelos, la interpretación de resultados y la evaluación de si se han descubierto nuevos patrones o se han respondido adecuadamente las preguntas planteadas.

El trabajo se realizará en grupos de **cinco personas**. Para su desarrollo, los integrantes deberán coordinarse fuera del horario de clases, ya sea de forma presencial o utilizando plataformas como Discord, Google Meet, Google Hangouts, WhatsApp o herramientas colaborativas como Google Docs/Slides. Se recomienda realizar al menos una o dos reuniones semanales para discutir avances y asignar tareas. Es fundamental que todos los miembros del grupo participen activamente en el estudio y contribuyan al informe final, que deberá ser editado en conjunto antes de su entrega.

### **Estructura y Evaluación del Proyecto**

El proyecto se evaluará en tres hitos, cada uno con un informe y una presentación. Además, cada hito contará con **una sesión de trabajo presencial obligatoria** durante el horario de cátedra. 

* **Hito 1**: Selección y exploración de un **conjunto de datos**, planteamiento de preguntas y problemas.

* **Hito 2**: Propuesta de **experimentos** y presentación de **resultados preliminares**. 

* **Hito 3**: Presentación de **resultados de todos los experimentos propuestos**.

El informe es incremental y deberá presentarse en formato de página web (HTML), puede ser utilizando Jupyter Notebook exportado a HTML o usando otra herramienta.

### **Plazos y Penalizaciones**

Los equipos cuentan con un margen de una semana para retrasos en la entrega del informe, con una penalización de 1 punto menos por cada día de atraso en la calificación final. Las ausencias en las sesiones de trabajo serán penalizadas por 0.3 puntos en la nota del hito correspondiente. 

 

# Hito 1

Cada grupo debe elegir un **dataset real**, ya sea público o privado para realizar su proyecto semestral (ver sugerencias [aquí](https://github.com/dccuchile/CC5205/blob/master/sugerencias_proyecto.md), pero incluso pueden recolectarlo Uds. mismos, u obtenerlo de otra fuente, la elección es libre). 

En esta etapa, los estudiantes deben presentar sus avances iniciales en  
	**A. Presentación presencial y**  
	**B. Informe**   
que deben ser enviados vía Tareas en la plataforma **U-Cursos**. A continuación, se detallan los contenidos solicitados y los criterios de evaluación.

### **Contenidos:** No olvidar ningún punto:

#### **1\. Motivación/Problema**

* ¿Cuál es el contexto general del tema/problema/datos de estudio?  
* ¿Por qué es interesante analizar estos datos?

#### **2\. Exploración de Datos (EDA)**

* Principales características del dataset (cantidad de registros, descripción de los atributos, estadísticas de resumen, visualizaciones, etc.).  
* Posible necesidad de agregar datos o fusionar tablas de diferentes granularidades.  
* Detectar posibles inconsistencias (datos faltantes, duplicados, etc.) y preprocesamiento necesario. 

#### **3\. Preguntas**

A partir del análisis exploratorio y su motivación original, formular preguntas relevantes para la minería de datos y que se puedan vincular a la problemática planteada, donde puedan argumentar que responderlas tenga alguna utilidad para alguien.

Ejemplos:

* ¿Es posible predecir la variable X en función de Y, Z y K?  
* ¿Existen grupos de datos con comportamientos similares?

Las preguntas deben ser útiles y responderse mediante técnicas de aprendizaje automático (clasificación, regresión, clustering). **No se aceptan preguntas triviales que puedan responderse con simples correlaciones u otras técnicas exploratorias.** La idea es que los resultados de su exploración los ayuden a formular buenas preguntas. La gran diferencia entre una pregunta que se puede responder con exploración y otra que necesita técnicas de minería de datos, es que éstas últimas requieren la construcción de modelos que encuentren relaciones entre múltiples atributos y/o ejemplos. 

**El mínimo número de preguntas es 3 y debe haber al menos (sujeto a los datos) una que se aborde con técnicas de aprendizaje supervisado (ej: clasificación, regresión) y una de aprendizaje no supervisado (ej: clustering). Si no entienden la idea general de esas técnicas, por favor pregunten.** 

Opcionalmente, pueden plantear **hipótesis** basadas en estudios previos o intuiciones del equipo. Una hipótesis (de manera muy simplificada), es una creencia actual o resultado esperado asociada a sus preguntas. Por ejemplo: la literatura sugiere que los países latinoamericanos se comportan de manera más similar a los africanos que a los europeos respecto al criterio X, entonces esa será la hipótesis para esa pregunta. En ciertos casos, el objetivo es refutar la hipótesis actual mediante el análisis de datos. 

Sean conscientes que puede que sus datos actuales no permitan responder alguna de sus preguntas. En ese caso, pensar si es posible conseguir un dataset complementario que haga que esa pregunta sí pueda ser respondida. Si eso no es factible, descarten la pregunta.

***Ejemplo:** Supongamos que tenemos una dataset de reviews de cervezas, donde cada cerveza es evaluada con una nota por cada usuario que la consumió. Adicionalmente, nuestro dataset contiene columnas que describen el tipo de cerveza (pale ale, ipa, etc.), su grado alcohólico, país de origen, si es de cebada o trigo, marca, año de elaboración, entre otros.*

***Motivación:** podríamos comentar que actualmente el mercado de cervezas artesanales está creciendo, donde más y más personas están produciendo sus propios productos dado el consumo por año per cápita, la facilidad de entrar al mercado, etc.* 

***Exploración de datos:** dado que cada cerveza tiene una puntuación por usuario, podríamos mostrar el promedio de ranking por cerveza, así como su distribución usando boxplot. También cuánto cada usuario ha hecho un review a una cerveza, o el número de cervezas por país y su respectivo ranking de manera agregada. Uno podría, por ejemplo, observar que algunas cervezas podrían tener bajo o alto ranking por alguna razón que tal vez (a simple vista), no tengamos muy clara, o estadísticamente no sea fácil de deducir.* 

***Preguntas y problemas:** en base a nuestra motivación y análisis exploratorio, podrían surgir ciertas inquietudes que se ven representadas en los datos. Por ejemplo, nos haría re-pensar que tal vez hay características en los datos que nos permita, conocer por ejemplo, que ciertas cervezas con específicas cualidades podrían tener mejor (o peor) aprobación en el mercado. Por ende, preguntas que se pueden desprender serían algunas como estas:*

* *¿Existen características específicas de las cervezas que permitan tener mejor o peor aprobación del público?*

* *¿Sería posible conocer el ranking (aproximado) de una nueva cerveza que entra al mercado considerando sus características?*

* *¿Es posible encontrar grupos de cervezas (rating en común o similares) a partir de las cualidades de cada cerveza?*

**A. Presentación (Presencial \- 3 minutos)**

- **Contenido de la presentación: motivación/problema, EDA, preguntas.** Entregable: Presentación en formato PPT o PDF.

- **Calidad de la presentación: preparación del grupo, claridad en la exposición, manejo del tiempo, diapositivas):** Es importante que construyan una narrativa para su presentación. Traten de contar una historia, que cada parte se conecte con la anterior. Eviten mostrar cosas de manera aislada. Es muy probable que tengan que replantear lo que van a contar en una etapa anterior en base a lo que encontraron en una fase siguiente. Por ejemplo: puede que al diseñar las preguntas se den cuenta que faltó hacer algo en la exploración. En ese caso refinan su exploración para que su historia final quede más sólida.

**B. Informe en formato web: Extensión máxima equivalente a 5 páginas impresas (pueden previsualizar su HTML en modo impresión para verificar el largo). Debe ser enviado en un archivo que contenga todo lo necesario para su visualización.** El informe debe contener la información de la presentación de manera más detallada. Al final del informe se debe crear:

- Una sección donde mencionen cuál fue la **contribución** exacta de cada miembro al proyecto (ej. John Doe estuvo a cargo de la limpieza de datos y del análisis presentado en las tablas xx y xx, también redactó la sección xx del informe).   
- Una sección sobre el **uso de IA**, donde detallen de manera transparente, en los casos que aplique, qué herramientas utilizaron y para qué tareas específicas (ej. corrección de redacción, generación de código de visualización, etc.), especificando las indicaciones dadas (incluir los prompts en anexos). 

Estas dos secciones no se cuentan en el largo del informe, sin embargo, deben ocupar máximo 1 página adicional. Pueden incluir referencias bibliográficas sin límite de espacio. A su vez, gráficos o tablas que no sean relevantes pueden ir en anexos. Se debe incluir el **código fuente** del trabajo (por ej. generar la página usando jupyter notebook incluyendo el código, o poner enlaces a sus scripts). Mientras más reproducible el trabajo, mejor. El código no se cuenta en el largo máximo siempre que esté colapsado o en anexos.

**Estructura:**

1) Introducción: plantear el problema y la motivación  
2) Exploración de datos  
3) Preguntas  
4) Contribuciones del equipo  
5) Declaración de uso de inteligencia artificial

		Referencias bibliográficas  
		Anexos: Espacio para material complementario (descripción detallada de los atributos de los datos, códigos, tablas o gráficos secundarios). No se contabiliza dentro del límite de extensión y su lectura es opcional, es decir, el informe debe entenderse sin necesidad de revisarlo.

# Hito 2

El objetivo de este hito es abordar los problemas identificados en el Hito 1, mejorar la exploración de datos y preguntas (en especial debilidades señaladas en la corrección). También, desarrollar una propuesta metodológica de los experimentos de minería de datos a realizar en su proyecto en relación a las preguntas y metas planteadas, y llevar a cabo al menos un experimento de esta propuesta. En detalle:

1. #### **Mejoras hito 1:** 

* Ahora que veremos a detalle las técnicas de Minería de Datos, se espera que puedan refinar sus preguntas y alinearlas con lo que permiten hacer las herramientas.   
* Incluir datos (o datasets) que puedan complementar (o aportar más valor) a responder las preguntas del Hito 1\. Esto significa que algunas preguntas podrían no responderse con los datos explorados inicialmente, implicando agregar más columnas (o filas).   
* Mejorar la fase exploratoria para incorporar nuevas preguntas y/o fuentes de datos.   
* Es posible que su dataset actual no cumpla las características mínimas para el proyecto, por lo que esta instancia permite replantear la factibilidad de continuar con estos datos y buscar un problema nuevo. En este caso, se recomienda que los grupos se pongan en contacto con el equipo docente para evaluar la situación de manera personalizada.   
* Incluir las sugerencias del equipo docente para consolidar el hito 1\. 

2. #### **Propuesta metodológica experimental:** 

Describir la metodología experimental para responder todas sus preguntas. Esto incluye:

* Preprocesamiento adicional necesario.  
* Plantear los modelos y técnicas de minería de datos a utilizar.  
* Plantear las métricas y técnicas de evaluación de los resultados. Complementar el análisis cuantitativo (métricas) con análisis cualitativo.   
* Justificación de cada decisión tomada. Esta propuesta es un contrato que deberán luego llevar a cabo en el Hito 3\. ARGUMENTEN TODAS SUS DECISIONES.

Ejemplo: para responder la pregunta X vamos a agregar los datos por país, luego reduciremos las dimensiones usando las técnicas Z y K o combinaremos los atributos H y L mediante una suma, para luego aplicar clustering. Elegiremos la mejor solución de clustering comparando los algoritmos E, F, G y los compararemos con el método de visualización con diferentes números de clusters. La idea es que los resultados de este experimento nos permitirán responder la pregunta X mediante las métricas A, B, C. Den argumentos para **todas** las componentes de su metodología. ¿Por qué enfocarse en técnicas Z y K?, ¿Por qué evaluar con la métrica A, B? ¿Qué haremos si no encontramos resultados significativos? (por ejemplo probaremos clasificación).

Comentarios: 

* Si van a usar técnicas supervisadas (clasificación o regresión) se recomienda comparar varios modelos en sus experimentos (árboles, KNN, SVM, etc), así como hiperparámetros (pueden buscar los mejores valores usando herramientas como GridSearchCV). Similar con técnicas no supervisadas.   
* Si van a usar técnicas de resampling por tener clases desbalanceadas (oversampling de clase minoritaria, subsampling de clase mayoritaria, SMOTE), **no transformen sus datos de testing**.   
* Con técnicas supervisadas también es importante que analicen la **importancia de las características de entrada** (cuáles influyen más en la predicción de la variable objetivo).   
* Para experimentos con técnicas de clustering es muy importante hacer un **análisis cualitativo de sus clusters**. No es suficiente con detectar clusters. Pueden mirar algunos ejemplos por cluster (podrían ser los más representativos o centrales) y tratar de entender qué es lo que representan. También, agregar las características de los ejemplos de cada cluster. Se espera que traten de ponerle un nombre a sus clusters. Recuerden que el clustering debe evaluarse, veremos técnicas para hacerlo.  
* A veces es posible etiquetar manualmente una muestra de sus datos para poder aplicar técnicas de clasificación. Si no tienen etiquetas, las pueden crear ustedes mismos.   
* Pueden usar técnicas de análisis de datos que ustedes conozcan o quieran aprender y no se enseñan en el curso. Ejemplo, trabajar con series de tiempo, procesamiento de imágenes, procesamiento de lenguaje natural, etc.

3. #### **Resultado Preliminar**

Implementar (en su totalidad) al menos uno de los experimentos planteados en la parte anterior y discutir sus resultados. Tengan en consideración que si hacen un experimento deben probar varios parámetros dentro de los cuales está el algoritmo (por ej. si usa clasificación debe comparar varios algoritmos diferentes en un mismo experimento) ¿Permiten estos resultados preliminares responder la pregunta correspondiente? Recuerden que para el hito 3 deberán implementar todos los experimentos. 

***Ejemplo:** Retomando el ejemplo de las cervezas del hito anterior.*

***Mejorar hito 1:** Encontramos un dataset que incluye el consumo per cápita de cerveza en el mundo, por lo que complementaremos el análisis con estos datos. Otro caso opuesto sería que una o más preguntas no pudieran ser respondidas. En estos casos se deberían replantear qué preguntas o problemas es posible responder con el análisis exploratorio, incorporando nuevas fuentes o cambiando el dataset. En este último caso, se espera que los grupos se contacten con el equipo docente para ver el caso personalmente.* 

***Propuesta metodológica experimental:*** 

* *En el dataset existen cervezas sin ranking o que algunos ranking no están en una unidad estándar. Por lo tanto, pre-procesaremos los datos para limpiar los registros sin nota y estandarizaremos los valores de ranking en 2 escalas (cualitativo y cuantitativo).*  
* *Aplicaremos transformaciones al precio ya que este considera diferentes unidades, de modo de estandarizarla en una sola (CLP por ejemplo).*   
* *Extraeremos características del texto de los reviews, por lo que representaremos de forma vectorial el texto para entender si este puede (o no) entregar mayor información para las tareas planteadas.*   
* *Dado que nuestras preguntas 1 y 2 son de carácter predictivo, nos focalizaremos en clasificación, donde proponemos utilizar nuestro dataset para crear un modelo que permita estimar el ranking de una cerveza (escala cualitativa, por ejemplo: excelente, bueno, aceptable, malo, muy malo) a partir de un conjunto de 50 características.*   
* *Para evaluar la calidad de la clasificación compararemos diversos algoritmos (haciendo búsqueda de mejores hiperparámetros), utilizaremos las métricas tradicionales como F1, precision y recall, aplicando k-fold cross validation o un particionado de 80-20 para entrenamiento y testeo respectivamente.*  
* *También aplicaremos técnicas de clustering para encontrar de manera natural si las características de nuestro dataset son suficientes para encontrar grupos de cervezas similares (pregunta 3).*   
* *Probaremos múltiples combinaciones en el número de clúster así como distintos enfoques de clustering (particional y jerárquico). Ocuparemos P y Q heurísticas/técnicas para estimar los mejores parámetros de los distintos modelos.*   
* *También probaremos usando distintos subconjuntos de atributos al hacer clustering para evaluar si los ejemplos se agrupan de manera distinta.*   
* *Para visualizar los clusters en 2 dimensiones, probaremos A y B técnicas de reducción de dimensionalidad de los datos.*  
* *Para evaluar los clusters, utilizaremos el enfoque visual así como también la estimación de métricas tales como cohesión y separación.*

***Resultado Preliminar:** Aplicar técnicas de clustering a mis cervezas (K-means, y Jerárquico Aglomerativo), evaluar y discutir los resultados, incluyendo el análisis descriptivo de clusters.*

**A. Presentación (Presencial \- 3 minutos):** 

- **Presentación en formato PPT o PDF que resuma la idea general del proyecto, propuesta experimental y resultados del experimento realizado.**

- **Calidad de la presentación: preparación del grupo, claridad en la exposición, manejo del tiempo, diapositivas**.

**B. Informe en formato web: extensión máxima equivalente a 8 páginas impresas (donde 5 corresponden al hito 1 y 3 al hito 2\). Estructura:**

1) Introducción: plantear el problema y la motivación  
2) Exploración de datos  
3) Preguntas  
4) Propuesta metodológica experimental  
5) Experimento preliminar (implementación y análisis de resultados)  
6) Contribuciones del equipo  
7) Declaración de uso de inteligencia artificial  
8) Referencias bibliográficas  
9) Anexos

# **Hito 3**

El objetivo de este hito es presentar los resultados de los experimentos propuestos en el Hito 2\. En la presentación final, deberán resumir su trabajo destacando las conclusiones basadas en los resultados obtenidos, las lecciones aprendidas y las posibles líneas de trabajo futuro.

**A. Presentación (Presencial \- 7 minutos): Presentación en formato PPT o PDF.**

#### **Motivación y Objetivos Principales**

* Resumir el tema/problema de estudio. Motivando su importancia.  
* Explicar los objetivos principales del trabajo.

#### **Preguntas y Problemas Abordados**

* Exponer las preguntas que guiaron el análisis.  
* Justificar cómo estas preguntas se relacionan con los objetivos.

#### **Datos**

* Información **más relevante** obtenida de la exploración de datos (por ej: datos faltantes, estadísticas relevantes, eliminación de atributos, etc). 

#### **Experimentos y Resultados Relevantes**

* Describir los experimentos realizados y sus resultados.  
* Relacionar cada experimento con la pregunta o hipótesis que busca responder.  
* Explicar si los resultados obtenidos confirman o refutan la hipótesis. Recuerden que obtener resultados negativos es totalmente válido.   
* Complementar el análisis cuantitativo (métricas obtenidas) con análisis cualitativo:   
  * visualizaciones,   
  * ejemplos de casos donde los modelos aciertan o fallan,   
  * asignación de nombres a los clusters en caso de clustering, etc…  
* Destacar hallazgos clave y su relevancia.

#### **Futuras Direcciones**

* Identificar mejoras o líneas de trabajo futuro basadas en los conocimientos adquiridos.  
* Proporcionar recomendaciones para futuras investigaciones sobre el problema analizado.

#### **Calidad General de la Presentación**

* Preparación del grupo, claridad y coherencia en la exposición, manejo del tiempo, diapositivas.  
* Presentar los contenidos de manera estructurada y conectada, evitando mostrar información de forma aislada. Es fundamental construir una narrativa clara para la presentación. Cada parte debe conectar con la anterior y contar una historia. Es muy probable que tengan que replantear lo que van a contar en una etapa anterior en base a lo que encontraron en una fase siguiente.

**B. Informe en formato web: máximo 15 páginas en el cuerpo y cantidad ilimitada en anexos.** El informe debe ser lo más reproducible posible, incluyendo el código utilizado para generar estadísticas y análisis. Se recomienda que el código esté colapsado en anexos o enlazado en la web del grupo. **Contenido del Informe**

1. **Extensión y mejora del reporte (en formato web) del grupo**, detallando:

   * Todos los pasos desarrollados.

   * Resultados obtenidos.

   * Interpretaciones y análisis de resultados (cuantitativo y cualitativo).

2. **Citas a fuentes externas**

   * Incluir referencias a recursos reutilizados (código, datasets, metodologías previas).

   * Diferenciar claramente las contribuciones originales del grupo. En caso de reutilizar recursos externos indicar claramente cuáles son sus contribuciones originales (serán evaluados en base a eso).

3. **Conclusiones finales y planificación futura**

   * Reflexionar sobre los hallazgos obtenidos.

   * Plantear posibles mejoras o extensiones del trabajo.

4. **Contribuciones del equipo**

   * Explicitar el rol y aportes de cada miembro.

5. **Declaración de uso de inteligencia artificial**

   * Seguir lineamientos indicados en el Hito 1\.		

**Importante:** El cuerpo docente se reserva el derecho de reunirse con ciertos grupos o integrantes específicos para que expliquen el proyecto. Todos los miembros deben estar completamente familiarizados con el trabajo realizado y ser capaces de defenderlo. Es importante que se expliquen entre Uds. los experimentos que hicieron, sólo así podrán sacar conclusiones relevantes del trabajo completo.


# **Sesiones de Trabajo Obligatorias**

Para facilitar el desarrollo del proyecto y garantizar un avance sólido, se realizarán **tres sesiones de trabajo obligatorias** en la sala de clases, donde los equipos deberán asistir con sus computadores. Durante estas sesiones, los profesores de cátedra y los auxiliares estarán presentes para brindar apoyo y resolver dudas en tiempo real.

Estas sesiones tienen como objetivo proporcionar orientación práctica y asegurar que los grupos puedan abordar cada hito con una base sólida.

**Primera sesión (Exploración de datos y planteamiento de preguntas)**

* Revisión y discusión del dataset seleccionado.  
* Apoyo en la aplicación de técnicas de exploración de datos.  
* Asesoría en la formulación de preguntas relevantes para la investigación.  
* **Venir con**:   
  * Proposiciones de datasets  
  * Exploración de datos   
  * 5 Preguntas de investigación, para fijar 3 de ellas 

**Segunda sesión (Definición de preguntas y metodología experimental)**

* Evaluación de las preguntas planteadas y su viabilidad.  
  * Discusión sobre la metodología experimental para abordar las preguntas.  
  * Revisión de estrategias de preprocesamiento y selección de técnicas de minería de datos.  
  * Discusión y retroalimentación de resultados preliminares.  
  * **Venir con**:   
    1. Un dataset definido  
    2. Exploración de datos hecho   
    3. 3 Preguntas de investigación con metodología asociada para resolverlas    
    4. Experimentos preliminares 

**Tercera sesión (ejecución de experimentos e interpretación de resultados)**

* Apoyo en la implementación de los experimentos definidos en el Hito 2\.  
  * Análisis de los resultados obtenidos y orientación en su interpretación.  
  * Revisión de estrategias para mejorar los experimentos o ajustar preguntas si es necesario.  
  * **Venir con**:   
    1. Resultados de los experimentos para las 3 preguntas  
    2. Proposición de análisis de los modelos y de los datos 

Se espera que **cada equipo llegue preparado con avances y preguntas concretas para aprovechar al máximo las sesiones**.
