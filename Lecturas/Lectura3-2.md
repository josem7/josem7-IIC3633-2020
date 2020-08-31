## Evaluating Recommendation Systems

### Resumen

Este paper se concentra en como comparar diversos algoritmos recomendadores usando métodos de evaluación en vez de bench marks. Ellos proponen 3 entornos distintos, el primero, un entorno offline, el segundo un entorno donde se le pide a los usuarios usar el sistema en un entorno controlado y el tercero, donde los usuarios utilizan el sistema sin saberlo.

Luego proponen diversos métodos para evaluar distintas propiedades de los sistemas recomendadores. Ellos consideran métodos desde los más comunes como MAE, RMSE, precision, recall, etc. Hasta métodos para evaluar la privacidad, confianza del usuario en el sistema, escalabilidad, etc.

## Critica

Es bueno que usan una diversidad de entornos ya que cada uno tiene sus pros. En primer lugar, el entorno offline es el más simple de hacer. Luego, el entorno controlado provee la mayor cantidad de información y por último el entorno real es como verdaderamente se desempeñaría el sistema si este fuera utilizado.

Ellos entran en gran detalle en los pros y cons que pueden tener diversos entornos y los posibles riesgos de hacer experimentos en estos, como sugerir respuestas correctas en cuestionarios, etc.

Otro buen punto es que ellos proponen una hipótesis, controlan variables y ven que tan generalizable es. Esto es muy útil ya que hace que los experimentos sean más creíbles y estén apuntados a responder una pregunta en particular.

Interesante que consideren variados métodos estadísticos para corroborar que los resultados no se deben simplemente a la suerte o a otros factores no considerados y proponen como mejorar los diversos test hechos estadísticamente.

Muy bueno que consideren una diversidad de tests hechos para obtener información de distintas propiedades de los sistemas recomendadores como privacidad, escalabilidad, confianza, etc.
