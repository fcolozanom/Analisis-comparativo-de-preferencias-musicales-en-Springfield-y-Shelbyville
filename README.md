# Análisis-comparativo-de-preferencias-musicales-en-Springfield-y-Shelbyville
Este proyecto analiza datos de transmisión de música en dos ciudades, Springfield y Shelbyville, para identificar diferencias en preferencias musicales y actividad de usuarios en diferentes días y momentos. El objetivo es informar decisiones basadas en datos y estrategias de marketing específicas para cada ciudad.

# 1  Introducción 
Como analista de datos, tu trabajo consiste en analizar datos para extraer información valiosa y tomar decisiones basadas en datos. Esto implica diferentes etapas, como la descripción general de los datos, el preprocesamiento y la prueba de hipótesis.

Siempre que investigamos, necesitamos formular hipótesis que después podamos probar. A veces aceptamos estas hipótesis; otras, las rechazamos. Para tomar las decisiones correctas, una empresa debe ser capaz de entender si está haciendo las suposiciones correctas.

En este proyecto, compararás las preferencias musicales de las ciudades de Springfield y Shelbyville. Estudiarás datos reales de transmisión de música online para probar las hipótesis a continuación y comparar el comportamiento de los usuarios y las usuarias de estas dos ciudades.

# 1.1  Objetivo:
Prueba tres hipótesis:

1.- La actividad de los usuarios y las usuarias difiere según el día de la semana y dependiendo de la cuidad.
2.- Los lunes por la mañana, los habitantes de Springfield y Shelbyville escuchan géneros distintos. Lo mismo ocurre con los viernes por la noche.
3.- Los oyentes de Springfield y Shelbyville tienen preferencias distintas. En Springfield prefieren el pop, mientras que en Shelbyville hay más personas a las que les gusta el rap.

# 1.2  Etapas
Los datos del comportamiento del usuario se almacenan en el archivo /datasets/music_project_en.csv. No hay ninguna información sobre la calidad de los datos, así que necesitarás examinarlos antes de probar las hipótesis.

Primero, evaluarás la calidad de los datos y verás si los problemas son significativos. Entonces, durante el preprocesamiento de datos, tomarás en cuenta los problemas más críticos.

Tu proyecto consistirá en tres etapas:

Descripción de los datos
Preprocesamiento de datos
Prueba de hipótesis

# 1.3  Reto
En este proyecto, preparamos un pequeño reto para ti. Incluimos un nuevo tipo de estructura de datos: las marcas temporales. Las marcas temporales son muy comunes y merecen una atención adicional. Más adelante en el programa, aprenderás mucho sobre ellas. Sin embargo, por ahora las trataremos como simples strings. Necesitamos marcas temporales en este proyecto para poner a prueba una de nuestras hipótesis. No te preocupes, te ayudaremos con esto. Tu nivel de conocimientos actual será suficiente para abordarlo.

# Observaciones
1.- ¿Qué tipo de datos tenemos a nuestra disposición en las filas? ¿Y cómo podemos entender lo que almacenan las columnas? 
Los tipos de datos que tenemos a nuestra disposición son Objects (objetos). Para entender lo que almacenan las columnas: 'userID' — identificador del usuario o la usuaria; 'Track' — título de la canción; 'artist' — nombre del artista; 'genre' — género musical; 'City' — ciudad del usuario o la usuaria; 'time' — hora exacta en la que se reprodujo la pista; 'Day' — día de la semana.

2.- ¿Hay suficientes datos para proporcionar respuestas a nuestras tres hipótesis, o necesitamos más información? 
Si, considero que se cuenta con suficiente informacion para darle respuesta a las hipotesis.

3.- ¿Notaste algún problema en los datos, como valores ausentes, duplicados o tipos de datos incorrectos? 
Tiene valores duplicados y ausentes

4.- Encontramos variaciones en la escritura del género hiphop que podrían generarnos problemas al analizar la información puesto que tendríamos valores incorrectos. En la función se utilizó el bucle for para iterar sobre la lista de géneros incorrectos y reemplazarlos con el género correcto. Luego, se llamó a la función proporcionando la lista de géneros incorrectos ['hip', 'hop', 'hip-hop'] y el género correcto 'hiphop'. El resultado de esta operación fue que los géneros incorrectos fueron reemplazados por 'hiphop' en la columna 'genre' del DataFrame. Asegurando la uniformidad en la representación del género 'hiphop' corrigiendo las variaciones de escritura.

5.- Comente si la primera hipótesis es correcta o debe rechazarse. Explicar tu razonamiento. 
Dado que los números de canciones reproducidas son mucho mayores en Springfield que en Shelbyville en los tres días, es evidente que los patrones de consumo de música difieren entre las dos ciudades. Por lo tanto, la primera hipótesis es correcta, ya que, existen diferencias en la forma en que los usuarios y las usuarias de Springfield y Shelbyville consumen música.

6.- Comente si la segunda hipótesis es correcta o debe rechazarse. Explica tu razonamiento.
Si tenemos que:
Lunes por la mañana: En Springfield, los géneros más reproducidos son: pop, dance, electronic, rock. En Shelbyville, los géneros más reproducidos son: pop, dance, rock, electronic. 

Viernes por la noche: En Springfield, los géneros más reproducidos son: pop, rock, dance, electronic. En Shelbyville, los géneros más reproducidos son: pop, electronic, rock, dance. 

Podemos deducir que los géneros más reproducidos en ambos momentos del día son bastante similares entre las dos ciudades y no hay una diferenciación clara que sugiera que los ciudadanos de Springfield están escuchando géneros muy diferentes de los de Shelbyville en estos momentos específicos, podríamos considerar que la segunda hipótesis no está respaldada por estos resultados.

6.- Comente si la tercera hipótesis es correcta o debe rechazarse. Explica tu razonamiento.
Basándonos en los datos obtenidos, no hay evidencia de que la tercera hipótesis sea cierta ya que ambas ciudades tienen los géneros "pop", "dance", "rock", "electronic" y "hiphop" como los géneros más reproducidos.

# Conclusiones 
La primera hipótesis afirma que existen diferencias en la forma en que los usuarios de Springfield y Shelbyville consumen música. Esta hipótesis se confirma ya que los datos muestran que los patrones de consumo son significativamente distintos entre las dos ciudades. Los números de canciones reproducidas en Springfield son mucho mayores que en Shelbyville en los tres días considerados.

La segunda hipótesis plantea que los ciudadanos de Springfield y Shelbyville tienen preferencias de género musical distintas durante ciertos momentos del día. Sin embargo, al analizar los géneros más reproducidos en ambos momentos específicos (lunes por la mañana y viernes por la noche), no se encuentran diferencias significativas entre los géneros más populares en ambas ciudades. Por lo tanto, la segunda hipótesis no está respaldada por los resultados.

La tercera hipótesis sugiere que los ciudadanos de Shelbyville tienen una preferencia por la música rap, mientras que los de Springfield se inclinan hacia el pop. Sin embargo, al observar los géneros más reproducidos en ambas ciudades, se evidencia que ambas comparten los géneros "pop", "dance", "rock", "electronic" y "hiphop" como los más populares. Por lo tanto, no hay suficiente respaldo en los datos para afirmar que existe una preferencia clara por un género en una ciudad sobre la otra.