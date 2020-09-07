## Document Clustering Based On Non-negative Matrix Factorization

### Resumen
Este paper propone un nuevo método para hacer agrupamiento de grandes volúmenes de documentos con el objetivo de poder hacer búsquedas y navegación de manera efectiva. Esta técnica está basada en la factorización matricial del contenido del documento.

Dentro de los beneficios de este nuevo método se encuentra el hecho de que para textos hace más sentido que el tema de este se obtenga por suma de sus posibles tópicos subyacentes, este método no asume independencia entre estos temas subyacentes y la dirección semántica latente coincide con los grupos donde estos documentos son clasificados.

Este luego testea su modelo propuesto en 2 sets de datos TDT2 y REUTERS cada uno con distintas características, evalúan sus resultados utilizando accuracy (AC) y normalized mutual information metric (MI). Por último, ellos presentan sus resultados y muestran una mejora significativa con respecto a otros.

### Crítica

Me parece bueno que en los trabajos previos proponga críticas a los métodos que se han utilizado eso si estas críticas están basadas más en la lógica que en pruebas concretas ya que no hace referencia a ningún paper detallando estas críticas.

El método de optimización es bastante bueno y comúnmente usado lo que asegura convergencia en un óptimo, ellos también tratan el hecho de que pueden existir múltiples soluciones y también mencionan la complejidad de este método lo que es muy positivo al momento de comparar dos algoritmos.

No me gusta el hecho de que en sus tests hayan excluido ciertos datos del test set ya que esto podría llevar a "cherry pick" los datos para que el algoritmo propuesto funcione de mejor manera, otro punto criticable de esto es que los documentos en la vida real pueden tener esta gran variación y un algoritmo que planea agrupar documentos tiene que ser capaz de abordar este tipo de situaciones.

Me gustaría que mostraran como fueron construidos los métodos con los que comparan su algoritmo para ver si efectivamente intentaron hacer los otros métodos de la mejor manera posible y de esta forma obtener una comparación más justa.
