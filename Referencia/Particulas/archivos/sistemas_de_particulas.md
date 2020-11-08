# Sistemas de Partículas

Antes de usar partículas es necesario crear sistemas de partículas. Un sistema de partículas es como un contenedor donde se colocan las partículas y emisores. Se pueden tener tantos sistemas como sea necesario, sin embargo, es mejor mantener una cantidad reducida ya que los sistemas, emisores y partículas ocupan memoria y tener demasiados puede causar problemas.

Este es un ejemplo de uso. Imagine que necesita algún efecto que aparezca sobre un instancia, y otro efecto que aparezca debajo de todas instancias, podría crear dos sistemas con profundidades diferentes para tener el efecto deseado.

1.  ## Funciones para preparar sistemas de partículas
    
    Ya que un sistema de partículas es un recurso creado dinámicamente, se debe almacenar su índice en una variable para hacer referencia al sistema en las siguientes funciones. Es muy importante destruir los sistemas cuando ya no son necesarios, de lo contrario se podría usar un exceso de memoria que bajaría el rendimiento del juego. Cabe resaltar que los sistemas de partículas vivirán por siempre después de que son creados, incluso si su índice no se guarda en una variable. Al cambiar de room o reiniciar el juego, los sistemas de partículas permanecerán activos. Esta es otra razón por la que deben ser destruidos cuando ya no son necesarios.
    
    A continuación se listan las funciones básicas para preparar sistemas de partículas:
    
    *   `part_system_create()`
    *   `part_system_exists()`
    *   `part_system_clear()`
    *   `part_system_depth()`
    *   `part_system_position()`
    *   `part_system_destroy()`
    *   `part_particles_clear()`
    *   `part_particles_count()`
2.  ## Funciones para dibujar sistemas de partículas
    
    Las instancias de partículas normalmente se actualizan en cada Step y se dibujan en base a los parámetros que las definen. Sin embargo, algunas veces es necesario controlar cuándo y cómo se actualiza un sistema y cómo se dibuja. Para ello, GMS provee las siguientes funciones:
    
    *   `part_system_automatic_update()`
    *   `part_system_automatic_draw()`
    *   `part_system_update()`
    *   `part_system_drawit()`
    *   `part_system_draw_order()`
3.  ## Crear partículas directamente
    
    Se pueden usar emisores para crear instancias de partículas en estallidos o en un flujo contante, pero en muchas situaciones los emisores no son necesarios y es mejor crear las partículas directamente con las siguientes funciones:
    
    *   `part_particles_create()`
    *   `part_particles_create_colour()`