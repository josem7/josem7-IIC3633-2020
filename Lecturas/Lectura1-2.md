## Funk SVD

Funk SVD es un algoritmo recomendador que nace en el contexto de la competencia de Netflix "Netflix Price".
Este método busca en primer lugar descomponer a las películas y usuarios en una cantidad de características (42 en este caso) a partir de los ratings que dieron los usuarios. Uno podría pensar en estas características como que tan de acción, romance, SC-FI, etc. es cada película y usuario, aunque en realidad es un poco más complejo que eso. El problema es que hay valores que faltan por lo tanto se usan métodos como descenso de gradiente para tener una buena estimación de qué podrían ser estos valores.

Dentro de los posibles problemas que se encuentran están el sobre ajuste que a veces puede producir el método de descenso de gradiente, para esto ellos fijan un número máximo de iteraciones o ciclos para definir cada una de las características. El hacer esto tiene el problema de que es importante el número con el que uno comienza por lo que hace falta una forma de estimar este número inicial.

Otro posible problema es la escalabilidad de este método si bien la competencia consistía en muchos datos y el computador lo hacía bastante rápido (7.5 segundos) no estoy seguro como se comportaría en un sistema donde todo el tiempo están entrando usuarios y es necesario hacer nuevas predicciones para cada nuevo usuario.

Por último, este sistema necesita de datos explícitos como user rating y no es capaz de inferir información de datos que no están de manera tan explícita, de donde se podría inferir mucha información para el sistema recomendador.
