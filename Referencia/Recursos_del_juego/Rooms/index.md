## Rooms

Las _rooms_ en GameMaker: Studio son los lugares (escenas) donde todo sucede en tu juego. Debes tener por lo menos una habitación en cualquier juego para que funcione, pero en general necesitarás muchas más. Esta sección tiene todas las funciones GML relacionadas con las _rooms_ e información sobre ellas al igual que para establecerles ciertas propiedades. Cabe decir que aquellas funciones relacionadas con cambiar las propiedades de las _rooms_ **nunca** deben ser ejecutadas desde la misma habitación, sino que deben ser ejecutadas primero desde una instancia en otra habitación.  

1.  ## Información de _rooms_
    
    Las siguientes funciones y variables globales son usadas para obtener información básica sobre la _room_:  
      
    *   `room_exists()`
    *   `room_first`
    *   `room_last`
    *   `room_previous()`
    *   `room_next()`
    *   `room`
    *   `room_speed`
    *   `room_height`
    *   `room_width`
    *   `room_persistent`
    *   `room_caption`
    *   `room_get_name()`
2.  ## Moverse entre _rooms_
    
    Las siguientes funciones son usadas para moverse entre las _rooms_:  
      
    *   `room_goto()`
    *   `room_goto_next()`
    *   `room_goto_previous()`
    *   `room_restart()`
3.  ## Crear y cambiar _rooms_
    
    Las siguientes funciones son usadas para crear _rooms_ y cambiar propiedades de las _rooms_:  
      
    **NOTA:** Estas funciones **no pueden ser usadas en la misma room**, de lo contrario pueden producirse errores y comportamientos impredecibles.  
      
    *   `room_add()`
    *   `room_duplicate()`
    *   `room_assign()`
    *   `room_instance_add()`
    *   `room_instance_clear()`
    *   `room_tile_add()`
    *   `room_tile_add_ext()`
    *   `room_tile_clear()`
    *   `room_set_background()`
    *   `room_set_background_colour()`
    *   `room_set_height()`
    *   `room_set_width()`
    *   `room_set_persistent()`
    *   `room_set_view()`
    *   `room_set_view_enabled()`