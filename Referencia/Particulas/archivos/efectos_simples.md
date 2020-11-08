# Efectos Simples

La forma más fácil de crear partículas en un juego es usar el mecanismo de efectos simples. Los efectos se crean usando un sistema de partículas predefinido. Es un método rápido para dibujar efectos gráficos sin tener que preocuparse por los detalles (como manejo de memoria). Simplemente se especifica el tipo de efecto, la posición donde debe ser creado, el tamaño, y finalmente el color, entonces GMS hace todo el trabajo.

Las siguientes funciones permiten crear los efectos de partículas predefinidos.

*   `effect_create_below()`
*   `effect_create_above()`
*   `effect_clear()`

También hay un grupo de constantes para cada tipo de efecto.

*   [Anexo: Constantes para efectos simples](anexo_constantes_para_efectos_simples.html)

Aunque estos efectos están limitados en alcance y personalización, pueden crear buenos efectos con muy poco esfuerzo. Por ejemplo, al crear una pequeña nube de humo en cada Step, bajo un misil en movimiento, se genera un rastro de humo bastante convincente. Aunque usted sea un experto en partículas conviene recordar que estos efectos existen, ya que pueden ahorrar tiempo algunas veces.