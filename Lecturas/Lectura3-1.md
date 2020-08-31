## Performance of Recommender Algorithms on Top-N Recommendation Tasks

### Resumen:

Este paper trata de proponer nuevas formas de evaluar top-N recommendation task. En este se argumenta que las formas tradicionales como MAE y RMSE dan tan solo una aproximación de la tarea de top-N y proponen métricas como recall y precision.

Ellos dividen el set de datos en dos sets entrenamiento M y test T (este solo contiene ratings de 5 estrellas), ellos usan el data set de Netflix y el de Movielense para esto. Luego para cada ítem que el usuario evaluó con 5 estrellas se eligen 1000 ítems de manera random y se intenta que el ítem número 1 en la lista ordenada sea el que el usuario evaluó con 5 estrellas, luego ellos proponen un top-N si el ítem evaluado con 5 estrellas está dentro de los primeros N ítems es un acierto si no es un fallo.

Luego comparan como distintos tipos de algoritmos comúnmente usados se comportan con este test, siendo el algoritmo que proponen ellos el que obtiene mejor resultado tanto considerando los ítems más populares como no considerándolos.



## Critica

Para mí no es bueno el hecho de que el test set se debe elegir de manera adecuada para evitar sesgos en la métrica de precisión. Otra área que mejoraría a futuro es que en el set de test no solamente tener los datos de ítems con 5 estrellas. Asumen que los 1000 ítems puestos de manera random para cada ítem evaluado con 5 estrellas no son de interés para el usuario cosa que tal vez no es así.

Me parece interesante que mencionen como los ítems más populares se llevan la mayor cantidad de evaluaciones, a ellos no les interesa recomendar ítems populares si no que recomendar más variedad lo que es interesante.

Otro aspecto positivo es que ellos atacan el problema que los sistemas recomendadores basados en RMSE contienen solo ítems que el usuario evaluó, pero no consideran aquellos ítems que el usuario no evaluó

Algo que no me parece ni bueno ni malo pero interesante es que explican los distintos tipos de sistemas recomendadores, lo encuentro bueno porque da una mayor claridad, pero lo encuentro malo ya que alargó innecesariamente el paper quizás lo pudieron haber incluido en un anexo
