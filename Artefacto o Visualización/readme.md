![Cabezote](../Imágenes/Cabezote.png)

# Visualización

Como producto final del proyecto, se desarrolló una tablero de visualización en ***Power Bi*** que permite explorar todas las solicitudes de restablecimiento y reportes de vulneración de derechos a niñas, niños y adolescentes presentadas al ICBF entre enero de 2015 y mayo de 2021. Igualmente, muestra los resultados del modelo de *Machine Learning* entrenado para poder clasificar estas peticiones de acuerdo a su veracidad y gravedad, lo cual se pleantea como una importante herramienta para los equipos de Defensoría de Familia en busca de priorizar la constatación y verificación de las situaciones reportadas.

Este tablero se puede consultar [en este enlace](https://app.powerbi.com/view?r=eyJrIjoiOTUxMjRkYzItOGJlNy00OGY0LThjYjUtYWI3YmQ2YzA1YmM4IiwidCI6IjNkOTJhNWYzLWJjN2EtNGE3OS04YzVlLTVlNDgzZjc3ODliZiIsImMiOjR9) o haciendo clic en la siguiente imagen.

[<img src="../Imágenes/Tablero_Inicio.png">](https://app.powerbi.com/view?r=eyJrIjoiOTUxMjRkYzItOGJlNy00OGY0LThjYjUtYWI3YmQ2YzA1YmM4IiwidCI6IjNkOTJhNWYzLWJjN2EtNGE3OS04YzVlLTVlNDgzZjc3ODliZiIsImMiOjR9)


A continuación se hace una breve descipción de cada una de las pantallas disponibles en el tablero, que de forma general permiten filtrar las peticiones por: regional y centro zonal a la que se direccionó, año y mes en que se registró, el canal de recepción, el motivo de ingreso, el tipo (solicitud de restablecimiento de derechos -SRD- o reporte de amenaza o vulneración -RAVD-) y palabra clave contenida en la descripción.

* [Descripción general de las peticiones](#Descripción-general-de-las-peticiones)
* [Análisis por regional y tiempo (año, mes día y hora)](#Análisis-por-regional-y-tiempo)
* [Estado de las peticiones](#Estado-de-las-peticiones)
* [Caracterización de niños, niñas y adolescentes afectados](#Caracterización-de-niños-niñas-y-adolescentes-afectados)
* [Análisis por centro zonal](#Análisis-por-centro-zonal)
* [Triage de solicitudes de restablecimiento y reportes de vulneración de derechos](#Triage-de-solicitudes-de-restablecimiento-y-reportes-de-vulneración-de-derechos)


## Descripción general de las peticiones
En esta vista se puede analizar el total de peticiones entre enero de 2015 y mayo de 2021, de acuerdo a las palabras más frecuentes que se registran en la descripción del hecho, el año en que sucede y el tipo de peticionario que reporta la situación al ICBF (el mismo afectado, un familiar, un anónimo, la policía o fiscalía, alguien asociado a una entidad de salud o educativa, entre otros).

![Tablero Descripcion General](../Imágenes/Tablero_General.png)

## Análisis por regional y tiempo
Mediante esta visualización se puede analizar las regionales a las que se direcciona el mayor número de peticiones a la par de los momentos en lo que se presentan de forma más frecuente de acuerdo al año, mes, día de la semana y hora.

![Tablero regional y tiempo](../Imágenes/Tablero_Temporal.PNG)

## Estado de las peticiones
Permite conocer el número de solicitudes de restablecimiento y reportes de amenaza o vulneración de derechos que han ameritado la apertura de un Proceso Administrativo de Restablecimiento de Derechos (PARD), si este ha sido un PARD no Institucional o un PARD Institucional, si no se pudo constatar el reporte o si se reportó que era falso.

![Tablero Estado de las peticiones](../Imágenes/Tablero_EstadoPeticiones.png)

## Caracterización de niños, niñas y adolescentes afectados
De acuerdo a la información entregada por el peticionario al momento de comunicarse con el ICBF, esta vista hace una desagregación de acuerdo a características de los niños, niñas o adolescentes a los que se reporta han sido vulnerados sus derechos. Esta caracterización incluye variables como sexo, edad, pertenencia étnica, zona de residencia (urbana o rural), discapacidad o víctima de desplazamiento forzado.

![Tablero Caracterizacion de los afectados](../Imágenes/Tablero_CaracterizacionAfectado.png)

## Análisis por centro zonal
Esta última vista del total de peticiones permite ver los centros zonales a los que se direcciona la mayor cantidad, permitiendo igualmente observar en qué año y mes son más frecuentes, si se abre un PARD, el motivo de ingreso por el que se abre un PARD y las palabras clave que se encuentran de forma más frecuente en la descripción de la petición.

![Tablero Centro Zonal](../Imágenes/Tablero_CentroZonal.png)

## Triage de solicitudes de restablecimiento y reportes de vulneración de derechos
En esta sección se encuentra un prototipo de visualización que serviría a los equipos de Defensoría de Familia a priorizar las peticiones de acuerdo con su veracidad y gravedad. Tomando cada una de las peticiones registradas en 2021, se muestra cuál es la predicción del modelo de *Machine Learning*  (el cual se explica en la sección de [`Algoritmos y Entrenamiento`](../Algoritmos%20y%20Entrenamiento/) sobre como se clasificaría: si es un reporte que se predice tendrá una constatación Sin Definir, Fallida o Falsa o, si por el contrario, es un reporte que se predice será Verdadera y ameritará o no la apertura de un PARD.

![Tablero Triage Clasificacion de reportes](../Imágenes/Tablero_PrediccionTriage.png)

