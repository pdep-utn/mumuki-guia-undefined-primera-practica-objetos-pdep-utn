¡Muy bien!

Este ejercicio tiene muchos lugares para aplicar _polimorfismo_: de `delfina` hacia las consolas y/o videojuegos, y de los videojuegos hacia las consolas. Recordemos que una solución con _polimorfismo_ implica abstraerse en algún punto de la lógica concreta de cada objeto de un conjunto para poder tratar indistintamente uno u otro. Para lograr esto, es necesario que esos objetos **entiendan los mismos mensajes** (no todos, sino los necesarios para poder tratarlos _polimórficamente_). Esto aparece:

- Al calcular la diversión que otorga un videojuego. En algunos casos eso depende de la consola que se use (para `mario` y `pokemon`) mientras que en otros no (como `arkanoid`). Si queremos tratarlos _polimórficamente_ (como al hacer que `delfina` juegue) será necesario que el mensaje sea el mismo (esto incluye nombre y parámetros), así que si algunos del grupo necesitan algún parámetro (como podría ser la consola) entonces todos lo deberían recibir (por más que en algunos casos no se use).
- Al usar una consola. Si bien `portatil` sufre un efecto al ser usada, `play` no. Entonces, **¿es necesario que el objeto `play` tenga un método `usar()` que no hace nada?** Si queremos tratarlas _polimorficamente_ (como al hacer que `delfina` juegue), entonces sí. Como es indiferente qué consola se esté usando, ambos objetos son posibles candidatos de recibir el mensaje `usar()` y, para el caso particular de `play`, **NO es lo mismo tener un método que no hace nada en vez de no tenerlo: en el primer caso el objeto entiende el mensaje y no hace nada, en el segundo no se entiende el mensaje y _el programa se rompe_**.


Además, todo este esquema es posible de manejar dado que cada objeto tiene _responsabilidades_ bien definidas. Hay que tener cuidado, por ejemplo, al calcular la diversión que otorga un videojuego, que en la mayoría de los casos depende de dos objetos: el videojuego y la consola. Entonces, **¿a quién se le manda el mensaje, a la consola o al videojuego?**

Prestando atención, si bien la lógica necesita de ambos objetos, por cómo está planteado este caso, **el que define cómo se calcula la diversión es el videojuego**, y la consola (en realidad, su jugabilidad) es solamente un dato para resolver la ecuación. Así que lo mejor para saber qué cálculo hacer sería **mandarle el mensaje para saber la diversión que otorga al videojuego** (pasándole la consola por parámetro si es necesario) y aprovechar el _polimorfismo_.


Por último, para reflexionar: **¿cómo modelaste que `portatil` tenga _batería baja_? ¿qué se guarda como atributo? ¿la jugabilidad la calcula en el momento de usarse o se la guarda previamente?**
