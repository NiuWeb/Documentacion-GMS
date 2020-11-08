# draw_sprite_tiled_ext

Dibuja un sprite con las propiedades dadas y lo repite hasta rellenar la vista.

## Síntaxis

  
```gml  
draw_sprite_tiled_ext(sprite, subimg, x, y, xscale, yscale, colour, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar.|  
subimg|El número de la subimagen del sprite a dibujar (0 es la primera).|  
x|La posición horizontal donde dibujar el sprite.|  
y|La posición vertical donde dibujar el sprite.|  
xscale|La escala horizontal del sprite (1 es el tamaño original).|  
yscale|La escala vertical del sprite (1 es el tamaño original).|  
colour|El color con el cual mezclar el sprite (use c_whtie para dibujar normalmente).|  
alpha|La opacidad del sprite (1 es totalmente opaco).|  

## Descripción

Esta función es una mezcla entre `draw_sprite_tiled()` y `draw_sprite_ext()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_sprite_tiled_ext(sprite_index, image_index, x, y, 2, 2, c_red, 0.5);  
```  
Se dibujará repetidamente el sprite actual de la instancia con el doble de tamaño, color rojo y 50% de opacidad, hasta llenar la vista de la sala.