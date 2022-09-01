Queremos modelar la épica batalla entre un valiente gato y un vil ratón:

<iframe width="420" height="315"
src="https://www.youtube.com/watch?v=6oLPCTH4nWE">
</iframe>


Esta batalla se basa en infinitas persecuciones de `tom` intentando atrapar a `jerry`, pero `jerry` siempre logra escapar, ya sea por sus propios medios, ó a veces con ayuda de su `robotRaton`, a quien usa como señuelo.

![robot-raton](https://s-media-cache-ak0.pinimg.com/236x/1f/13/17/1f1317e6a5887547544c0f1c721d1fa8.jpg)

En particular, nos interesa saber saber si `tom` es más veloz que un ratón, o sea, si su velocidad es mayor que la velocidad del ratón. Tener en cuenta que 

  * la velocidad de `tom` se calcula como 5 + (su energía / 10).
  * la velocidad de `jerry` se calcula como 10 menos su peso.
  * la velocidad del `robotRaton` es siempre de 8 unidades.
  * `tom` tiene inicialmente `80` unidades de energía, y `jerry`, `3` unidades de peso.
 
Además, queremos hacer que `tom` corra a un ratón. Cuando `tom` corre un ratón: 

  * consume tanta energía como 0.5 * su velocidad * distancia entre ambos, y
  * su posición actual pasa a ser igual a la del ratón. 
  * `tom` está inicialmente en la posición `0`, `jerry` en la `10` y el `robotRaton` en la `12`.

> Declarar los objetos necesarios de forma que
> 
> 1. Todos entiendan el mensaje `velocidad()`
> 2. `tom` entienda el mensaje `esMasVeloz` pasándole algún ratón por parámetro
> 3. `tom` entienda el mensaje `correrA` pasándole algún ratón por parámetro

Para pensar:

> ¿`velocidad` es un **método o atributo** de `tom`? ¿Y de `jerry`?

> ¿Hace falta que el `robotRaton` tenga peso?

> ¿Qué mensajes debería entender un nuevo ratón para poder ser perseguido por `tom`? Si te animás, ¡agregá uno inventado por vos!
