Queremos modelar cómo varía la diversión de `delfina`, una niña a la que le gusta jugar videojuegos.

Las consolas que tiene disponibles son:

- Una `play` que otorga una jugabilidad de 10 unidades
- Y una `portatil` que otorga una jugabilidad de 8, a menos que tenga la _batería baja_, en ese caso solamente 1 unidad


Queremos hacer que `delfina` juegue a un videojuego. Cuando esto sucede:

- primero `delfina` aumenta su nivel de diversión según cuánto otorgue el juego
- Y luego se le asigna un uso a la consola

Cuando alguien usa la `play` no pasa nada, pero cuando la `portatil` se usa queda con _batería baja_.


`delfina` siempre comienza con un nivel de diversión de 0 y tiene muchos videojuegos, por ahora nos interesa modelar:

- `arkanoid`: otorga una diversión de 50 unidades
- `mario`: si la consola tiene la jugabilidad necesaria (mayor que 5) otorga una diversión de 100 unidades, caso contrario 15
- `pokemon`: la diversión que otorga se calcula como 10 * la jugabilidad de la consola


> Se pide:
>
> 1. Las consolas entiendan el mensaje `jugabilidad()` que indica cuánta jugabilidad otorga.
> 2. Las consolas entiendan el mensaje `usar()` que provoca que la consola reciba un uso.
> 3. `delfina` entienda el mensaje `agarrar(consola)` para cambiar la consola que tiene en la mano.
> 4. `delfina` entienda el mensaje `jugar(videojuego)`.
> 5. `delfina` entienda el mensaje `diversion()` que indica su nivel de diversión.
