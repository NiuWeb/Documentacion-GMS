# draw_sprite_ext

Dibuja un sprite con propiedades personalizadas.

## Síntaxis

  
```gml  
draw_sprite_ext( sprite, subimg, x, y, xscale, yscale, rot, colour, alpha );  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar|  
subimg|El número de subimagen a dibujar (la primera subimagen es 0)|  
x|La posición horizontal en donde dibujar|  
y|La posición vertical en donde dibujar|  
xscale|La escala horizontal del sprite. 1 es el tamaño original.|  
yscale|La escala horizontal del sprite. 1 es el tamaño original.|  
rot|La rotación (en grados) del sprite|  
colour|el color con el que mezclar el sprite. Use `c_white` para dibujar normalmente.|  

## Descripción

De forma similar a `draw_sprite()`, esta función dibujará un sprite, pero en este caso con opciones adicionales para modificar su apariencia. Estas modificaciones **no afectan** al sprite original, sino solamente afectan a cómo se mostrará al momento de usar la función. También es posible utilizar las variables de sprites de cada instancia como argumentos de esta función.  
  

![](https://2.bp.blogspot.com/-IKeF989kXLs/WdLga0sFMKI/AAAAAAAAAig/ooiIJpQ9apgI8SHLLBoZ5SpCCewf3JuyQCLcBGAs/s1600/draw_sprite_ext.png)

  
  
**NOTA:** La mezcla de colores en la plataforma HTML5 es recomendada **sólo** cuando WebGL es activado, aunque de no estárlo, dicha mezcla seguirá funcionando normalmente. Sin embargo, sin WebGL todas las mezclas de color crean un sprite duplicado que se almacenará en la caché para usarse cuando sea neceesario. Esto está lejos de ser óptimo, y si se usan muchos cambios de color podría producirse una ralentización y bajón de rendimiento en el juego hasta que se active WebGL. Si usted no desea usar WebGL, también puede intentar modificar el tamaño del caché de sprites usando `sprite_set_cache_size()` e intentar limitarlo para mejorar el rendimiento.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_sprite_ext(sprite_index, image_index, x, y, image_xscale, image_yscale, image_angle, image_blend, image_alpha);  
```  
El anterior código permitirá dibujar el sprite actual de la instancia con las propiedades de ésta. En escencia funciona exactamente igual que `draw_self()`.