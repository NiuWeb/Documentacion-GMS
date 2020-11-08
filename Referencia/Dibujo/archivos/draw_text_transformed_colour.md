# draw_text_transformed_colour

Dibuja un texto con color, opacidad, escala y ángulo personalizados.

## Síntaxis

  
```gml  
draw_text_transformed_colour(x, y, str, xscale, yscale, angle, c1, c2, c3, c4, alpha);  
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
c1|El color de la ezquina superior izquierda del texto.|  
c2|El color de la ezquina superior derecha del texto.|  
c3|El color de la ezquina inferior derecha del texto.|  
c4|El color de la ezquina inferior izquierda del texto.|  
alpha|La opacidad del texto (1 es original).|  

## Descripción

Esta función es una mezcla entre `draw_text_colour()` y `draw_text_transformed()`

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_halign(fa_center);  
draw_set_valign(fa_middle);  
image_angle += 1;  
draw_text_transformed_colour(room_width / 2, room_height / 2, keyboard_string, 2, 2, image_angle, c_red, c_red, c_yellow, c_yellow, 0.5);  
```