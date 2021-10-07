![Cabezote](Imágenes/Cabezote.png)



# MODELO TRIAGE S.R.V.D
Este proyecto realiza procesamiento de lenguaje natural (NLP) sobre los textos e interacciones en chat de denuncias de vulneración de derechos de niños, niñas y adolescentes realizadas a través de los canales del ICBF, con el propósito de diseñar artefactos de priorización de verificaciones en campo u otras herramientas similares como artefactos de reacción inmediata, chatbots, etc.

## Tabla de contenidos

* [Descripción](#Descripción)
* [Objetivos](#Objetivo-general)
* [Tecnologías involucradas](#Tecnologíasinvolucradas)
* [Datos](#Datos)
* [Algoritmos y Entrenamiento](#AlgoritmosyEntrenamiento)
* [Artefacto o Visualización](#ArtefactoVis)

## Descripción

Anualmente el *Instituto Colombiano de Bienestar Familiar* **(ICBF)** recibe alrededor de **120 mil** denuncias asociadas a vulneraciones de derechos de niños, niñas y adolescentes, debido a esto usa gran parte de sus recursos en la verificación y constatación en campo de las mismas. Sin embargo, algunas de estas requieren ser priorizadas para minimizar el riesgo individual y familiar. 

En el marco de la Alianza Nacional contra la Violencia hacia Niñas, Niños y Adolescentes, el Instituto Colombiano de Bienestar Familiar (ICBF) ha trabajado en el desarrollo de modelos predictivos de vulneraciones que afectan a la niñez y adolescencia. La realización de estos modelos va en línea con el objetivo de “Crear las condiciones para anticipar y resolver las violencias y vulneraciones contra niñas, niños y adolescentes”, contenido en el Plan Nacional de Desarrollo 2018-2022. Este ha sido un trabajo conjunto realizado con el Departamento Nacional de Planeación (DNP) en el marco del Subsistema de Protección de Derechos, creado en el Plan Nacional de Desarrollo 2018-2022.

Pensando en esto, el *Grupo de Analítica Institucional* (GAI) del ICBF emprendió este proyecto para diseñar mecanismos que permitan automatizar la clasificación de riesgo de las denuncias y comprender el contexto en el que ocurren, a través del análisis sistemático de las descripciones de las denuncias mediante las técnicas de procesamiento de lenguaje natural. Este proyecto permitirá que el ICBF pueda pilotear mecanismos más eficientes de distribución de los recursos para la verificación en campo y constatación de las reportes de vulneración de los niños, niñas y adolescentes del país.

## Objetivo general

* Diseñar artefactos de priorización de verificaciones en campo u otras herramientas similares como artefactos de reacción inmediata, chatbots, etc, con base en el procesamiento de lenguaje natural (NLP) sobre los textos e interacciones en chat de denuncias de vulneración de derechos de niños, niñas y adolescentes realizadas a través de los canales del ICBF.

### Objetivos Especificos

* Realizar un análisis contextual de las denuncias de acuerdo con los tipos de violencias o vulneraciones de derechos de los que son víctimas los niños, niñas y adolescentes, mediante procesamiento de lenguaje natural de las descripciones de las denuncias que recibe el ICBF.

* Identificar variables y factores que permitan realizar predicción y etiquetado de los reportes de vulneración de derechos de acuerdo con su posible veracidad y gravedad.

* Diseñar un prototipo de artefacto que permita a los equipos del ICBF consultar los niveles de prioridad (pronosticados por el modelo) en la verificación y constatación en campo de las denuncias que reciben.


## Tecnologías Involucradas

En este apartado se encuentra una descripción de las tecnologias usadas por el grupo de analítica institucional del ICBF, además se presenta el **Diagrama de arquitectura**  que describe el orden y como están interrelacionadas dichas tecnologías en el desarrollo del presente modelo.

## Datos 

En esta sección el lector podrá encontrar tres carpetas:

* [`Diccionario`](Datos/Diccionario)

* [`Modelo`](Datos/Modelo)

* [`Muestra de Datos`](Datos/Muestra)


## Algoritmos y Entrenamiento

En la carpeta correspondiente se encuentra la *Metodología* y los cinco pasos principales involucrados en el desarrollo del Módelo Triage

1. Gestión de los datos
2. Procesamiento de lenguaje natural 
3. Entrenamiento de modelos de *Machine Learning*
4. Evaluación de resultados de los modelos y selección del mejor modelo
5. Triage/Clasificación de nuevas solicitudes

## Artefacto o Visualización

Una vez logrados los pasos anteriores, se mostrará las distintas vistas o tableros generados por medio de ***Power Bi*** de la clasificación de nuevas solicitudes que ingresan diariamente al ICBF obtenidas a partir del procesamiento del lenguaje natural y el modelo de predicción previamente entrenado.







