# Modelo de Regresión para predecir viajes en EcoBici y Clasificador de noticias
Trabajo Práctico 2 de la materia Laboratorio de Datos (2do cuatrimestre 2023) sobre un Modelo de Regresión para predecir viajes diarios en EcoBici y Clasificador de noticias reales y falsas de un dataset.


# Parte 1: Regresión
Elaborar un modelo de regresión para predecir el número de usos diarios del sistema de Ecobici. El dataset clima_ecobici contiene información registrada por la estación meteorológica del Aeroparque durante todos los días del 2022 y el número total de usos diarios de bicicletas del sistema Ecobici en la CABA. Las variables del dataset son:

&nbsp;&nbsp;&nbsp;&nbsp; • date: fecha <br>
&nbsp;&nbsp;&nbsp;&nbsp; • tavg: temperatura promedio (en grados Celcius) <br>
&nbsp;&nbsp;&nbsp;&nbsp; • tmin: temperatura mínima (en grados Celcius) <br>
&nbsp;&nbsp;&nbsp;&nbsp; • tmax: temperatura máxima (en grados Celcius) <br>
&nbsp;&nbsp;&nbsp;&nbsp; • prcp: precipitación (en mm) <br>
&nbsp;&nbsp;&nbsp;&nbsp; • wdir: dirección del viento <br>
&nbsp;&nbsp;&nbsp;&nbsp; • wspd: velocidad del viento (en km/h) <br>
&nbsp;&nbsp;&nbsp;&nbsp; • pres: presión atmosférica (en hPa) <br>
&nbsp;&nbsp;&nbsp;&nbsp; • n: número de bicicletas utilizadas <br>
Nota: Este dataset se construyó con todos los datos de usos del sistema Ecobici, no a partir del dataset reducido que se usó en el TP-1.

El modelo que tienen que proponer debe tener contener 2 de las siguientes variables predictoras:

&nbsp;&nbsp;&nbsp;&nbsp; • temperatura del día (promedio, mínima o máxima).<br>
 &nbsp;&nbsp;&nbsp;&nbsp; • si llueve o no llueve.<br>
&nbsp;&nbsp;&nbsp;&nbsp; • presión atmosférica.<br>
&nbsp;&nbsp;&nbsp;&nbsp; • velocidad del viento.<br>
 &nbsp;&nbsp;&nbsp;&nbsp; • si es día laborable o no laborable.<br>
Para construir el modelo sigan estos pasos: <br>

  &nbsp;&nbsp;&nbsp;&nbsp; 1. Realizar un análisis exploratorio que justifique la elección de las variables predictoras. <br>
 &nbsp;&nbsp;&nbsp;&nbsp; 2. Ajustar el modelo. <br>
 &nbsp;&nbsp;&nbsp;&nbsp; 3. Reportar adecuadamente el modelo resultante. Interpretar los coeficientes encontrados. <br>
 &nbsp;&nbsp;&nbsp;&nbsp; 4. Hacer visualizaciones apropiadas. <br>

 # Parte 2: Clasificación
El objetivo de este ejercicio es desarrollar un clasificador de noticias en “reales” o “fake-news”. El dataset contiene información sobre 150 noticias, algunas reales y otras falsas. Tienen una variedad de predictores pero vamos a trabajar sólo con tres:

&nbsp;&nbsp;&nbsp;&nbsp; • title_has_excl: variable binaria que indica si el título de la noticia tiene o no signos de exclamación. <br>
&nbsp;&nbsp;&nbsp;&nbsp; • negative: porcentaje estimado de palabras en el título que tienen connotaciones negativas. <br>
&nbsp;&nbsp;&nbsp;&nbsp; • title_words: número de palabras en el título. <br>
(La variable respuesta está en la variable type) <br>

1)  Realizar visualizaciones apropiadas para convencerse de que las variables predictoras podrían servir para clasificar las noticias en “reales” vs. “fake-news”.

2) Separar el dataset en un conjunto de entrenamiento y uno de prueba. Construir dos clasificadores (uno con k-NN y otro con un árbol de decisión) usando las tres variables mencionadas en 1. Justificar la elección de los parámetros del modelo (por ejemplo, el valor de k en k-NN). Reportar las matrices de confusión y accuracy de los modelos.

3) Supongamos que se publica un nuevo artículo que tiene un título de 15 palabras sin signos de exclamación y el 6% de sus palabras tienen connotaciones negativas. Calcular la probabilidad de que el artículo sea “fake-news”.
