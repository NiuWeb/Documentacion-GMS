# draw_sprite

Dibuja un sprite en la posición dada.

## Síntaxis

  
```gml  
draw_sprite(sprite, subimg, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar (es una constante de nombre o un número real).|  
subimg|La subimagen del sprite a dibujar (un número real).|  
x|La posición horizontal en donde dibujar el sprite.|  
y|La posición vertical en donde dibujar el sprite.|  

## Descripción

Esta función dibuja un sprite con una determinada imagen en la posición dada. Para el parámetro sprite puede usarse la variable `sprite_index` para dibujar el sprite actualmente asignado a la instancia, o bien puede usarse cualquier otro nombre de sprite (**NO** como cadena de texto).  
  
Lo mismo para la subimagen, puede usarse la variable `image_index` para dibujar un sprite con la subimagen actual **de la instancia** (no del sprite usado). Si el valor de la subimagen es mayor a la cantidad total de subimágenes del sprite menos 1, dicho valor se ajustará para quedar dentro del rango. Por ejemplo, si un sprite tiene 5 subimágenes (de 0 a 4) y se usa el número 5 como subimagen, éste será ajustado para dibujar la primera subimagen (índice 0). Las coordenadas toman en cuenta el origen del sprite.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_sprite(spr_Sol, 0, room_width/2, 128);  
```  
Se dibuja la primera subimaen del sprite _spr_Sol_ centrada horizontalmente en la sala, y a 128px del borde superior de la sala.