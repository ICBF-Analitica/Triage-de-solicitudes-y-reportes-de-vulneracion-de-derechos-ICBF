![Cabezote](Imágenes/Cabezote.png)



# MODELO TRIAGE S.R.V.D
Este proyecto busca construir un prototipo de consumo o visualización de un modelo de clasificación de las solicitudes de restablecimiento y reportes de amenaza y vulneración de derechos (en adelante, peticiones) que recibe el ICBF a través de sus distintos canales, que permita definir posteriormente el nivel de prioridad que deberían tener las verificaciones y constataciones en campo. Se basa en el entrenamiento de modelos usando variables numéricas, categóricas y features obtenidas a través del procesamiento de lenguaje natural (NLP) de las descripciones de las peticiones. La información que se toma en cuenta para el entrenamiento de los modelos proviene de características de los departamentos, de información descriptiva de los peticionarios y de los afectados, así como de algunas caracteristicas relevantes de la completititud de la petición y de la descripción del hecho.

## Tabla de contenidos

* [Descripción](#Descripción)
* [Objetivos](#Objetivo-general)
* [Tecnologías involucradas](Tecnologías%20Involucradas/)
* [Datos](Datos/)
* [Algoritmos y Entrenamiento](Algoritmos%20y%20Entrenamiento/)
* [Artefacto o Visualización](Artefacto%20o%20Visualización/)

## Descripción

El *Instituto Colombiano de Bienestar Familiar* **(ICBF)** recibe alrededor de **120 mil** reportes de amenaza y vulneración de derechos y solicitudes de restablecimiento de derechos  de niños, niñas y adolescentes, que demandan un gran esfuerzo institucional en la verificación y constatación en campo. Gran parte de ellas revisten un nivel de priorización alto debido a sus graves consecuencias sobre el bienestar individual y familiar, de manera que una herramienta que permita hacer una especie de "Triage" de las peticiones, constituye un gran aporte para el trabajo de las Defensorías de Familia del país. 

En el marco de la Alianza Nacional contra la Violencia hacia Niñas, Niños y Adolescentes, el Instituto Colombiano de Bienestar Familiar (ICBF) ha trabajado en el desarrollo de modelos predictivos de vulneraciones que afectan a la niñez y adolescencia. La realización de estos modelos va en línea con el objetivo de “Crear las condiciones para anticipar y resolver las violencias y vulneraciones contra niñas, niños y adolescentes”, contenido en el Plan Nacional de Desarrollo 2018-2022. 

Pensando en esto, el *Grupo de Analítica Institucional* (GAI) del ICBF emprendió este proyecto para diseñar mecanismos que permitan automatizar la clasificación de riesgo de las peticiones y comprender el contexto en el que ocurren, a través del análisis sistemático de las descripciones de las denuncias mediante las técnicas de procesamiento de lenguaje natural. Este proyecto permitirá que el ICBF pueda pilotear mecanismos más eficientes de distribución de los recursos para la verificación en campo y constatación de las reportes de vulneración de los niños, niñas y adolescentes del país.

## Objetivo general

* Diseñar un artefacto o prototipo de clasificación automatizada de las solicitudes de restablecimiento y reportes de amenaza y vulneración de derechos de niños, niñas y adolescentes, recibidas por el ICBF a través de diferentes canales.

### Objetivos Especificos

* Realizar un análisis contextual de las peticiones de acuerdo con los tipos de violencias o vulneraciones de derechos de los que son víctimas los niños, niñas y adolescentes, mediante procesamiento de lenguaje natural de las descripciones de las peticiones que recibe el ICBF.

* Identificar variables y factores que permitan realizar predicción y etiquetado de las solicitudes de restablecimiento o reportes de amenaza y vulneración de derechos. 

* Diseñar un prototipo de tablero de consumo de resultados del modelo de clasificación que permita a los equipos de Defensoría del ICBF consultar los niveles de prioridad (pronosticados por el modelo de acuerdo con su posible veracidad y gravedad) en la verificación y constatación en campo de las peticiones que reciben.


## Tecnologías Involucradas

En el apartado [`Tecnologías involucradas`](Tecnologías%20Involucradas/) se encuentra una descripción de las tecnologías usadas por el Grupo de Analítica Institucional (GAI) del ICBF. Además se presenta el **Diagrama de arquitectura**  que describe el orden y como están interrelacionadas dichas tecnologías en el desarrollo del presente proyecto.

## Datos 

En la sección [`Datos`](Datos) el lector encontrará información relevante sobre los datos utilizados en el entrenamiento del modelo, así como una muestra de datos a través de la cual se podrá adelantar una réplica parcial del ejercicio desarrollado por el Instituo. Los componentes encontrados allí son los siguientes: 

* [`Diccionario`](Datos/Diccionario)
* [`Modelo`](Datos/Modelo)
* [`Muestra de Datos comprimida en .zip`](Datos/datos_muestra_ICBF_Sandbox.zip)


## Algoritmos y Entrenamiento

En la carpeta [`Algoritmos y Entrenamiento`](Algoritmos%20y%20Entrenamiento/) se encuentra la *Metodología* y los cinco pasos principales involucrados en el desarrollo del Módelo Triage:

1. Gestión de los datos
2. Procesamiento de lenguaje natural 
3. Entrenamiento de modelos de *Machine Learning*
4. Evaluación de resultados de los modelos y selección del mejor modelo
5. Triage/Clasificación de nuevas solicitudes

## Artefacto o Visualización

El ICBF desarrolló un tablero o visualización que permite consumir los resultados de la clasificación predicha de las peticiones recibidas por el ICBF en ***Power Bi***. En este tablero se podrá consultar la clasificación de nuevas solicitudes que ingresan diariamente al ICBF obtenidas a partir del procesamiento del lenguaje natural y el modelo de predicción previamente entrenado. Mayor información sobre este desarrollo se puede encontrar en la carpeta [`Artefacto o Visualización`](Artefacto%20o%20Visualización/)

## Realizadores

Javier Rubio;
José Niño Muriel;
Johanna Lozano;
Campo E. Pinillos;
Luz Helena Trujillo;
Luigi Lizcano León;
Rafael Martínez
