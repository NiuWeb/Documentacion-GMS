# draw_text_transformed

Dibuja un texto con escala y ángulo personalizados.

## Síntaxis

  
```gml  
draw_text_transformed(x, y, str, xscale, yscale, angle);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal donde dibujar el texto.|  
y|La posición vertical donde dibujar el texto.|  
str|La cadena de texto a dibujar.|  
xscale|La escala horizontal del texto (1 es tamaño original).|  
yscale|La escala vertical del texto (1 es tamaño original).|  
angle|El ángulo del texto, en grados.|  

## Descripción

Esta función es similar a `draw_text()`, con la diferencia de que es posible escalar y rotar el texto a dibujar.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_halign(fa_center);  
draw_set_valign(fa_middle);  
image_angle += 1;  
draw_text_transformed(room_width / 2, room_height / 2, "¡HAS PERDIDO!", 2, 2, image_angle);  
```