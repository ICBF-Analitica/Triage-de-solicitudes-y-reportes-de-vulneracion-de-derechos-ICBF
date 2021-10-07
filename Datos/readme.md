![Cabezote](../Imágenes/Cabezote.png)

# DATOS

## Bases de datos

El siguiente modelo Entidad-Relación muestra las diferentes fuentes de información empleadas en el proyecto y las llaves que las relacionan para poder tener una base de datos consolidada con toda la información de las solicitudes y reportes de vulneración de derechos, que hacen posible el entrenamiento de un modelo de clasificación automatizada (Consulte el archivo .pdf en el siguiente enlace [`Modelo_relacional_peticiones.pdf`](Modelo/Modelo_relacional_peticiones.pdf). 

![modelo_relacional](../Imágenes/modelo_entidad_relacion.PNG)

En la sección `1. Gestión de los datos` de la carpeta [`Algoritmos y Entrenamiento`](../Algoritmos%20y%20Entrenamiento) se puede encontrar una descripción detallada de la forma en que estos datos fueron procesados.

##  Diccionario de datos

En la carpeta [`Diccionario`](Diccionario) se encuentra el archivo en formato Excel que contiene la descripción, y los posibles valores que toman cada una de las variables empleadas en el entrenamiento del modelo, así como en la construcción de la visualización.

###  Datos de muestra

Las fuentes de datos usadas por el ICBF contienen datos personales e información sensible, que hacen imposible compartir la totalidad de los datos o variables empleadas en el proyecto, acorde a la Ley de protección de datos personales (Ley 1581 de 2012). Para hacer posible una réplica del ejercicio desarrollado por el ICBF, se comparte una muestra anonimizada del 20% (196.858 registros) de los datos empleados para el entrenamiento de los distintos de modelos de *Machine Learning*. Estos datos, como puede inferirse, no contienen información personal o que permita la identificación de los individuos, pero permiten que los modelos puedan ser replicados por aquellos interesados en conocer más sobre el tema.

Estos datos se encuentran comprimidos en [`datos_muestra_ICBF_Sandbox.zip`](datos_muestra_ICBF_Sandbox.zip), el cual contiene cuatro archivos en formato `.parquet`:

* datos_modelo_sinDescripcion: Contiene las 30 variables explicativas empleadas para el entrenamiento de los modelos (13 numéricas y 17 categóricas) y también la variable objetivo llamada `VAR_OBJETIVO`.
* datos_modelo_Descripcion_tokenizer: Contiene 200 variables obtenidas a partir del preprocesamiento del campo `DescripcionPeticion` mediante el método de "Texto a secuencias", el cual es empleado para el entrenamiento de los modelos de redes neuronales.
* datos_modelo_Descripcion_tfidf: Contiene 300 variables obtenidas a partir del preprocesamiento del campo `DescripcionPeticion` mediante el método de "TF-IDF", el cual es empleado para el entrenamiento de los modelos de *Gradient Boosted Trees*.
* datos_modelo_Descripcion_wordembeddings: Contiene 100 variables obtenidas a partir del preprocesamiento del campo `DescripcionPeticion` mediante el método de *"Word Embeddings"*, el cual es empleado para el entrenamiento de los modelos de *Gradient Boosted Trees*.
