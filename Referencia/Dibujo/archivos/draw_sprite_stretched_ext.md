# draw_sprite_stretched_ext

Dibuja un sprite estirado con propiedades de color y opacidad.

## Síntaxis

  
```gml  
draw_sprite_stretched_ext(sprite, subimg, x, y, w, h, colour, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar|  
subimg|La subimagen del sprite a dibujar (0 es la primera subimagen)|  
x|La posición horizontal donde dibujar el sprite.|  
y|La posición vertical donde dibujar el sprite.|  
w|El tamaño horizontal del sprite|  
h |El tamaño vertical del sprite.|  
colour|El color con el cual mezclar el sprite (use c_white para dibujarlo normalmente).|  
alpha|La opacidad del sprite (1 es opacidad normal).|  

## Descripción

Esta función realiza el mismo trabajo que `draw_sprite_stretched()`, con la diferencia de que permite establecer un color de mezcla y opacidad.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_sprite_stretched_ext(sprite_index, image_index, x, y, sprite_width / 2, sprite_height / 2, c_white, 0.5);  
```  
Se dibuja el sprite actual de la instancia con la mitad de su tamaño original y una opacidad del 50%.