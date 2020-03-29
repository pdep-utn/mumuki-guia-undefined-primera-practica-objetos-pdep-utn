¡Muy bien! Pasaron todas las pruebas.

Este ejercicio plantea por un lado, el uso de _polimorfismo_ en como `tom` interactúa con los ratones. Por ejemplo, en el método `esMasVeloz` al esperar por parámetro cualquier ratón,  y _abstraer_ la idea un ratón genérico, trata indistintamente (_polimórficamente_) a cualquiera de los ratones del sistema.
Esto además permite:

- Mantener las _responsabilidades_ de los objetos. `tom` solamente se encarga calcular su velocidad y ver si es mayor que la del ratón, mientras que los ratones se encargan de calcular sus respectivas velocidades.
- Poder _extender_ el sistema fácilmente. Se puede agregar más ratones sin que ello involucre meterse en la lógica de `tom`.



Además hay que diseñar el modelado de los objetos, particularmente elegir qué variables son _atributos_ y cuáles _métodos de consulta_. Por ejemplo, el `peso` de `jerry` es una _variable independiente_ ya que **no depende de ningún otro valor y debemos recordarlo**, por lo que es necesario tenerlo como _atributo_. 
En cambio, su `velocidad` es una _variable dependiente_ ya que **se calcula a partir del peso**. En este caso es conveniente tener ese cálculo en un _método de consulta_.

_Para más información podés consultar [este artículo](http://wiki.uqbar.org/wiki/articles/oo-temporary-variable.html)._


Por último, es necesario que `tom` se envíe mensajes a él mismo, por ejemplo para conocer su velocidad. Recordá que `self` es una referencia que tienen todos los objetos hacia ellos mismos y sirve para auto-enviarse mensajes.

También es útil para _dividir en sub-tareas_. **¿Qué tan complejo te quedó el método `correrA` de `tom`?** Tal vez se pueda separar la lógica en varios métodos, ¡si es que ya no lo hiciste!
