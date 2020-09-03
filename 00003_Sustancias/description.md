Logan pesa 70 kilos. Y se sabe que el consumo de distintas sustancias le provoca distintas cosas. Pero tiene la gran ventaja de que cada sustancia que consume _reemplaza_ a la sustancia anterior. 

Hoy modelaremos tres sustancias:

* **clo2**: el dióxido de cloro provoca irritación en el esófago y en el estómago. Una persona con clo2 en su sistema tiene un rendimiento de 0.9 elevado a la dosis consumida, en centímetros cúbicos.
* **Tereré**: el tereré es diurético, laxante y estimulante del rendimiento. Una persona con tereré en su sistema tiene un rendimiento de 0.1 por cada centímetro cúbico de dosis. Sin embargo, nunca rinde menos que 1.
* **Cianuro**: el cianuro no favorece al rendimiento, sino que la persona luego de consumirlo queda como muerta, llena de abulia y de marasmo. Con cianuro, el rendimiento es siempre 0.

> 1. Hacer que Logan consuma cierta cantidad de una sustancia, con el mensaje `consumir(cantidad, sustancia)`
> 2. Conocer la fuerza de logan, mediante el mensaje `fuerza()`.

La fuerza de Logan se calcula como el rendimiento de la sustancia multiplicada por la inercia base de logan (5 kg*m/s) multiplicada por su peso.

> _No vale que la fuerza sea un atributo._
