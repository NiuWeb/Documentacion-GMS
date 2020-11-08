# draw_sprite_general

Dibuja una parte de un sprite con propiedades de color, escala y rotación modificables.

## Síntaxis

  
```gml  
draw_sprite_general(sprite, subimg, left, top, width, height, x, y, xscale, yscale, rot, c1, c2, c3, c4, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar .|  
subimg|El número de subimagen a dibujar (0 es la primera subimagen del sprite).|  
left|La posición horizontal (ezquina superior izquierda) desde donde dibujar el sprite|  
top|La posición vertical (ezquina superior izquierda) desde donde dibujar el sprite|  
width|El tamaño (horizontal) del área del sprite a dibujar|  
height|El tamaño (vertical) del área del sprite a dibujar|  
x|La posición horizontal en donde dibujar el sprite.|  
y|La posición vertical en donde dibujar el sprite.|  
xscale|La escala horizontal del sprite (1 es tamaño original).|  
yscale|La escala vertical del sprite (1 es tamaño original).|  
rot|El ángulo de rotación del sprite en grados.|  
c1|El color con el cual mezclar el área superior izquierda del sprite.|  
c2|El color con el cual mezclar el área superior derecha del sprite.|  
c3|El color con el cual mezclar el área inferior derecha del sprite.|  
c4|El color con el cual mezclar el área inferior izquierda del sprite.|  
alpha|La opacidad del sprite (1 es opacidad original).|  

## Descripción

Esta función combina las funciones `draw_sprite_ext()` y `draw_sprite_part()`, añadiendo algunas opciones de mezcla de color adicionales a cada ezquina del sprite.  
  
 **NOTA:** La mezcla de colores en la plataforma HTML5 es recomendada sólo cuando WebGL es activado, aunque de no estárlo, dicha mezcla seguirá funcionando normalmente. Sin embargo, sin WebGL todas las mezclas de color crean un sprite duplicado que se almacenará en la caché para usarse cuando sea neceesario. Esto está lejos de ser óptimo, y si se usan muchos cambios de color podría producirse una ralentización y bajón de rendimiento en el juego hasta que se active WebGL. Si usted no desea usar WebGL, también puede intentar modificar el tamaño del caché de sprites usando `sprite_set_cache_size()` e intentar limitarlo para mejorar el rendimiento.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_sprite_general(sprite_index, image_index, 8, 8, sprite_width-16, sprite_height-16, x, y, 2, 0.5, 180, c_white, c_white, c_black, c_black, 1);  
```  
El anterior código dibujará la subimagen actual del sprite asignado a la instancia, omitiendo un margen de 8px en el sprite. Además, tendrá el doble del tamaño horizontal original y la mitad del vertical, así como también una rotación de 180 grados. Por último, el sprite se dibujará con un degradado desde el color original hasta una silueta negra.