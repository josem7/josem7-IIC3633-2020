## Performance of Recommender Algorithms on Top-N Recommendation Tasks

### Resumen:

Este paper trata de proponer nuevas formas de evualuar top-N recommendation task. En este se argumenta que las formas tradicionales como MAE y RMSE dan tan solo una aproximación de la tarea de top-N y proponen métricas como recall y precision.

Ellos dividen el set de datos en dos sets entrenamiento M y test T (este solo contiene raitings de 5 estrellas), ellos usan el dataset de Netflix y el de Movielense para esto. Luego para cada item que el usuario evaluó con 5 estrellas se eligen 1000 items de manera random y se intenta que el item número 1 en la lista ordenada sea el que el usuario evaluó con 5 estrellas, luego ellos proponen un top-N si el item evaluado con 5 estrellas está dentro de los primeros N items es un acierto si no es un fallo.

Luego comparan como distintos tipos de algoritmos comunmente usados se comportan con este test, siendo el algoritmo que proponen ellos el que obtiene mejor resultado tanto considerando los items más populares como no considerandolos.



## Critica

Para mi no es bueno el hecho de que el test set se debe elegir de manera adecuada para evitar sesgos en la métrica de precision. Otra área que mejoraría a futuro es que en el set de test no solamente tener los datos de items con 5 estrellas. Asumen que los 1000 items puestos de manera random para cada item evaluado con 5 estrellas no son de interes para el usuario cosa que tal vez no es así.

Me parece interesante que mencionen como los items más populares se llevan la mayor cantidad de evaluaciónes, a ellos no les interesa recomendar itemes populares si no que recomendr más variedad lo que es interesante.

Otro aspecto positivo es que ellos atacan el problema que los sistemas recomendadores basados en RMSE contienen solo items que el usario evaluó pero no consideran aquellos items que el usuario no evaluó

Algo que no me parece ni bueno ni malo pero interesante es que explican los distintos tipos de sistemas recomendadores, lo encunetro bueno por que da una mayor claridad, pero lo encuentro malo ya que alarg innecesariamente el paper quizas lo pudieron haber incluido en un anexo
