¡Bien hecho!

En este ejercicio el _polimorfismo_ aparece cuando `logan` **utiliza las distintas sustancias** para conocer su rendimiento.

Cabe destacar que para lograrlo, las sustancias deben entender el mismo mensaje, incluyendo nombre **y parámetros**. Esto significa que si para conocer el rendimiento que algunas sustancias es necesario pasar algún parámetro en el mensaje (como la cantidad de la dosis para el `clo2` y `terere`) entonces todas las sustancias (incluyendo el `cianuro`) lo deberían esperar.


También hay que diseñar qué datos son _atributos_ y cuáles _métodos de consulta_ de `logan`. El enunciado pide la `fuerza`, y es necesario que esta **no** sea un atributo ya que es una _variable dependiente_, se obtiene de un cálculo que involucra el rendimiento de la sustancia, y la inercia y el peso de `logan`. Es mala práctica "guardarse" un valor que depende de otros para ser calculado.

_Para más información podés consultar [este artículo](http://wiki.uqbar.org/wiki/articles/oo-temporary-variable.html)._


Para reflexionar en base a la definición de `logan`:

- Al calcular la fuerza, ¿aparecen los nombre para las variables `inercia` y `peso` o están directamente sus valores? ¡Recordá que ponerle nombre a las cosas aumenta el nivel de abstracción!
- ¿Se podría tener la `inercia` y `peso` en métodos de consulta, **sin necesidad** de tenerlo en algún atributo?
- ¿Cuándo se calcula el rendimiento? ¿Se calcula en el momento de usarse para calcular la fuerza o se guarda el valor previamente? ¡Ambas formas son posibles!
