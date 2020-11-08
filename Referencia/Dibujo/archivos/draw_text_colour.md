# draw_text_colour

Dibuja un texto en la posición dada con una gradiente de color personalizada.

## Síntaxis

  
```gml  
draw_text_colour(x, y, str, c1, c2, c3, c4, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal en donde dibujar el texto.|  
y|La posición vertical en donde dibujar el texto.|  
str|La cadena de texto a dibujar.|  
c1|El color de la ezquina superior izquierda del texto.|  
c2|El color de la ezquina superior derecha del texto.|  
c3|El color de la ezquina inferior derecha del texto.|  
c4|El color de la ezquina inferior izquierda del texto.|  
alpha|La opacidad del texto (1 es original).|  

## Descripción

 Esta función es muy similar a `draw_text()`, con la diferencia de que es posible escoger manualmente cuatro colores distintos y una opacidad para el texto. Los colores y opacidad dados como parámetros tienen prioridad sobre el color y opacidad definidos con `draw_set_alpha()` y `draw_set_colour()`.  
  
**NOTA:** La mezcla de colores degradados no está disponible en la plataforma HTML5 a menos de que WebGL esté activado, aunque aún se podrán mezclar la opacidad y el primero de los colores dados si no lo está. Sin embargo, todas las mezclas de color que se realicen sin WebGL crearán una copia de la fuente que se almacenará en caché; esto podría ralentizar el rendimiento de tu juego si se utiliza sin control. Es posible también definir límite de almacenamiento en caché de las fuentes utilizando `font_set_cache_size()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_colour(c_white);  
draw_text(100, 100, "Puntos: ");  
draw_text_colour(100, 200, string(score), c_lime, c_lime, c_green, c_green, 1);  
```