# Funciones de dibujo

Cuando un objeto tiene un _sprite_ asignado a él, éste se dibujará sin necesidar de programar nada en el evento _Draw_. Sin embargo, existen muchas ocasiones en las que será necesario añadir otros elementos dentro de dicho evento. Esta sección presenta las funciones disponibles para dibujar los diferentes elementos. Desde figuras geométricas básicas, _sprites_, texto e incluso primitivas, superficies y 3D.  

1.  ## Formas básicas
    
    GameMaker: Studio cuenta con una colección de funciones disponibles para dibujar diferentes formas y figuras. Estas funciones sólo deben utilizarse dentro del evento _Draw_ de alguna instancia (es posible usarlas en otro evento, pero no se mostrará nada en pantalla) y permiten crear efectos únicamente gráficos, es decir que no poseen ningun tipo de evento de colisión por sí mismos. Todas estas funciones son afectadas por el color de dibujo, opacidad y modo de mezcla actuales.
    
    ### Relacionados
    
    *   `draw_point()`
    *   `draw_point_colour()`
    *   `draw_line()`
    *   `draw_line_width()`
    *   `draw_line_colour()`
    *   `draw_line_width_colour()`
    *   `draw_circle()`
    *   `draw_circle_colour()`
    *   `draw_rectangle()`
    *   `draw_rectangle_colour()`
    *   `draw_roundrect()`
    *   `draw_roundrect_colour()`
    *   `draw_roundrect_ext()`
    *   `draw_roundrect_colour_ext()`
    *   `draw_ellipse()`
    *   `draw_ellipse_colour()`
    *   `draw_triangle()`
    *   `draw_triangle_colour()`
    *   `draw_arrow()`
    *   `draw_button()`
    *   `draw_set_circle_precision()`
2.  ## Dibujo de texto
    
    En GameMaker: Studio, existe una colección de funciones disponibles para dibujar texto en distintas formas. Estas funciones permiten modificar el color, tamaño y otras propiedades del texto dinámicamente, pero en plataformas como HTML5 y dispositivos móviles, estas modificaiones pueden ralentizar el juego, o bien hacer que el texto se vea mal. Por ello, es más recomendable tener fuentes con distintos tamaños que redimensionar el texto con código, o bien tener fuentes de gran tamaño y **reducirlo** con código, pero esto último sólo cuando se necesiten dibujar piezas pequeñas de texto.
    
    ### Relacionados
    
    *   `draw_set_font()`
    *   `draw_set_halign()`
    *   `draw_set_valign()`
    *   `draw_text()`
    *   `draw_text_ext()`
    *   `draw_text_colour()`
    *   `draw_text_transformed()`
    *   `draw_text_ext_colour()`
    *   `draw_text_ext_transformed()`
    *   `draw_text_transformed_colour()`
    *   `draw_text_ext_transformed_colour()`
3.  ## Primitivas
    
    Una primitiva es un tipo de figura que se forma mediante la definición de diferentes puntos en la pantalla. Estas figuras pueden ser desde simples grupos de puntos, líneas e incluso triángulos, a la vez que pueden poseer propiedades como cualquier otra figura (color, alfa e incluso una textura asignada). Con estos elementos es posible crear efectos fascinantes en un videojuego 2D. Por ejemplo, es posible crear un rectángulo utilizando múltiples primitivas triangulares, asignarles una textura y modificar secuencialmente la forma de la primitiva para crear un efecto de bandera ondulante.  
    
    ### Relacionados
    
    *   `draw_primitive_begin()`
    *   `draw_primitive_begin_texture()`
    *   `draw_primitive_end()`
    *   `draw_vertex()`
    *   `draw_vertex_colour()`
    *   `draw_vertex_texture()`
    *   `draw_vertex_texture_colour()`
4.  ## Dibujo de sprites
    
    Cuando se le asigna un sprite a una instancia, GameMaker: Studio lo dibujará por defecto con las propedades definidas con las diferentes variables de sprites. Sin embargo, al añadir cualquier código en el evento Draw se está "tomando el control" y dándole a GameMaker: Studio las instrucciones de lo que debe dibujar exactamente. Esto significa que debes usar las funcioniones de dibujo para definir lo que se debe, cómo y dónde dibujar.  
      
    **NOTA:** Las propiedades que se definan con estas funciones no afectarán a los recursos reales del juego, son propiedades que se toman en cuenta únicamente para el momento de ejecutar dichas funciones.  
    
    ### Relacionados
    
    *   `draw_self()`
    *   `draw_sprite()`
    *   `draw_sprite_ext()`
    *   `draw_sprite_general()`
    *   `draw_sprite_part()`
    *   `draw_sprite_part_ext()`
    *   `draw_sprite_stretched()`
    *   `draw_sprite_stretched_ext()`
    *   `draw_sprite_pos()`
    *   `draw_sprite_tiled()`
    *   `draw_sprite_tiled_ext()`
5.  ## Dibujo de backgrounds
    
    Aunque en el editor de _Rooms_ existen opciones para dibujar backgrounds en pantalla, es más común dibujarlos utilizando código. Con este fin, _GameMaker: Studio_ tiene una serie de funciones que permiten dibujarlos de distintas maneras.  
      
    **NOTA:** Es importante que al añadir cualquier código dentro del evento _Draw_ de una instancia desactivará el dibujo automático del sprite de ésta, por lo que será necesario dibujar manualmente este sprite.
    
    ### Relacionados
    
    *   `draw_background()`
    *   `draw_background_ext()`
    *   `draw_background_part()`
    *   `draw_background_part_ext()`
    *   `draw_background_stretched()`
    *   `draw_background_stretched_ext()`
    *   `draw_background_tiled()`
    *   `draw_background_tiled_ext()`
    *   `draw_background_general()`
6.  ## Color y mezcla
    
    _GameMaker: Studio_ tiene la capacidad de manipular el color, opacidad y mezcla (_blending_) de todos los elementos que se dibujan en pantalla. Con estas funciones es posible separar un color en sus componentes (RGB o HSV), crear nuevos colores, manipular la opacidad e incluso modificar los modos de mezcla (_blend modes_) para cambiar cómo los diferentes elementos se dibujarán en pantalla. Además de estas funciones, existen varias constantes qe pueden ser utilizadas como colores base.  
    [Ver **Anexo: Constantes de colores**](archivos/Anexo_Constantes_de_color.html).  
    [Ver **Anexo: Manejo de colores**](archivos/Anexo_manejo_de_colores.html)  
    
    ### Relacionados
    
    *   `draw_set_colour()`
    *   `draw_get_colour()`
    *   `draw_set_alpha()`
    *   `draw_get_alpha()`
    *   `draw_clear()`
    *   `draw_clear_alpha()`
    *   `make_colour_rgb()`
    *   `make_colour_hsv()`
    *   `colour_get_red()`
    *   `colour_get_green()`
    *   `colour_get_blue()`
    *   `colour_get_hue()`
    *   `colour_get_saturation()`
    *   `colour_get_value()`

**NOTA:** La mezcla de colores es recomendada en la plataforma HTML5 **sólo** cuando el _WebGL_ está activo. Anque esta mezcla pueda realizarse aun sin _WebGL_, esto provocará que se cree una copia del _background_ (u otro recurso, como _sprites_) con las modificaciones de color hechas, almacenándoce en la caché. Esto es muy poco óptimo, y muchos cambios de mezcla de color ralentizará el rendimiento del juego. Si aún así usted no desea usar _WebGL_ y necesita realizar mezclas de color, puede considerar limitar el tamaño del caché de los sprites (y backgrounds) usando la función `sprite_set_cache_size()`.