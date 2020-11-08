# draw_sprite_part_ext

Dibuja una parte de un sprite con las propiedades dadas.

## Síntaxis

  
```gml  
draw_sprite_part_ext(sprite, subimg, left, top, width, height, x, y, xscale, yscale, colour, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar|  
subimg|El número de la subimagen a dibujar (0 es la primera subimagen).|  
left|La posición horizontal (ezquina superior izquierda) desde donde dibujar el sprite|  
top|La posición vertical (ezquina superior izquierda) desde donde dibujar el sprite|  
width|El tamaño (horizontal) del área del sprite a dibujar|  
height|El tamaño (vertical) del área del sprite a dibujar.|  
x|La posición horizontal donde dibujar el sprite.|  
y|La posición vertical donde dibujar el sprite.|  
xscale|La escala horizontal del sprite (1 es tamaño original).|  
yscale|La escala vertical del sprite (1 es tamaño original).|  
colour|El color con el cual mezclar el sprite (use c_white para dibujarlo normalmente).|  
alpha|La opacidad (1 es opacidad por defecto, 0 es totalmente transparente).|  

## Descripción

Esta función es similar a `draw_sprite_part()`, sólo que permite definir propiedades adicionales como la escala, color de mezcla y opacidad.  
  
**NOTA:** Cuando se dibuja un sprite con esta función, el origen del mismo será ignorado y todos valores de posición tomarán en cuenta la esquina superior izquierda de éste.  
  
**NOTA:** Esta función sólo puede usarse con sprites de mapa de bits. Sprites vectoriales o de Spine no funcionarán.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_sprite_part_ext(sprite_index, image_index, 4, 4, sprite_width - 8, sprite_height - 8, x, y, 0.5, 1, c_white, 0.5);  
```  
Se dbujará el sprite actual de la instancia dejando un margen de cuatro pixeles en cada borde del mismo. Además, su proporción horizontal se reducirá a la mitad y se verá con un 50% de opacidad.