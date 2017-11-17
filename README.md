# SistemasBasadosEnReglas
Los sistemas basados en reglas trabajan mediante la aplicación de reglas, comparación de resultados y aplicación de las nuevas reglas basadas en situación modificada. También pueden trabajar por inferencia lógica dirigida, bien empezando con una evidencia inicial en una determinada situación y dirigiéndose hacia la obtención de una solución, o bien con hipótesis sobre las posibles soluciones y volviendo hacia atrás para encontrar una evidencia existente (o una deducción de una evidencia existente) que apoye una hipótesis en particular.
https://es.wikipedia.org/wiki/Sistema_basado_en_reglas

# La aplicacion
En la aplicación debemos ingresar un conjunto de reglas y un conjunto de evidencias (verdaderas o falsas) y el motor de inferencia nos arrojara los valores de los objetos que logre inferir. Veamos un ejemplo. Tenemos las siguientes reglas en la base de conocimientos del motor de inferencia:

-X>Y;

-A>Y;

-B^C>W;

D>M;

A>Z;

M>Z;

W^-D>P;

-P^-C>R;

-R^-P>L;

-Y^-P>L;

Y le pasaremos las siguientes evidencias, que serán tomadas en el orden en el que aparecen:

A:flase;

C:false;

M:false;

W:flase;

Como resultado el sistema inferirá las siguientes conclusiones finales:

A: false

Y: true

C: false

M: false

D: false

W: false
