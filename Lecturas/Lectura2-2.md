## BPR: Bayesian Personalized Ranking from Implicit Feedback

En este paper se explora la idea de hacer un ranking de items personalizado a partir de feedback implícito.

Un posible problema es que asumen que si un usuario vio un item i él lo prefiere antes que todos los items que no vio, esta suposición es válida, pero existen muchos factores de por qué un usuario no vio que no son considerados acá (por ejemplo, no sabía que el item existía).

Un aspecto importante del método que proponen es que este es flexible y se puede aplicar en una gran cantidad de modelos a diferencia de otros con los que se compara.

Un aspecto que no me gustó es que para el dataset de Netflix ellos ven si es que un usuario es probable que le dé un rating a una película lo que no es lo mismo que si le gustó la película.

Otro aspecto bueno del paper es que nuevamente compara los costos del álgoritmo O(X) con otros métodos utilizado lo que te da una idea de la rapidez y escalabilidad del método.

En conclusión, el nuevo método propuesto funciona bastante bien para los 2 mejores modelos recomendadores de la época la pregunta es si efectivamente vale la pena esta pequeña mejora a costa de un método mucho más complejo.
