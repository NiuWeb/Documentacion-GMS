## Movimiento y colisiones

En el desarrollo de casi cualquier juego, llegará un punto en el que será necesario manejar el movimiento y la reacción de colisión de unas instancias frente a otras. Sin embargo, cada tipo de juego requerirá diferentes formas de manejar estas propiedades. Por ejemplo, en un juego de plataformas será necesario el uso de una gravedad e incluso fricción en el movimiento, mientras que un juego _top-down_ puede desarrollarse mejor usando sistemas relativos de coordenadas. Debido a esto, _GameMaker: Studio_ incluye muchas formas de mover una instancia y detectar colisiones entre éstas.  

1.  ## Movimiento
    
    En cualquier juego, el movimiento y las posiciones son de vital importancia, y por ello GameMaker: Studio tiene una completa colección de funciones para lidiar con cualquier situación de este tipo.
    
    ### Relacionados
    
    *   `direction`
    *   `friction`
    *   `gravity`
    *   `gravity_direction`
    *   `hspeed`
    *   `speed`
    *   `vspeed`
    *   `x`
    *   `xprevious`
    *   `xstart`
    *   `y`
    *   `yprevious`
    *   `ystart`
    *   `distance_to_object()`
    *   `distance_to_point()`
    *   `motion_add()`
    *   `motion_set()`
    *   `move_towards_point()`
    *   `move_bounce_all()`
    *   `move_bounce_solid()`
    *   `move_contact_all()`
    *   `move_contact_solid()`
    *   `move_outside_all()`
    *   `move_outside_solid()`
    *   `move_random()`
    *   `move_snap()`
    *   `place_snapped()`
    *   `move_wrap()`
2.  ## Colisiones
    
    1.  ## Colisiones sin máscara
        
        Existen ocasiones en las que será necesario comprobar un punto en algún área determinada, sin utilizar máscaras de colisión ni objetos, como por ejemplo comprobar si el mouse está dentro de una figura geométrica. La siguiente es una lista de las funciones que permiten realizar esto.
        
        ### Relacionados
        
        *   `point_in_rectangle()`
        *   `point_in_triangle()`
        *   `point_in_circle()`
        *   `rectangle_in_rectangle()`
        *   `rectangle_in_triangle()`
        *   `rectangle_in_circle()`