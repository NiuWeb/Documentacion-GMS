# draw_text_ext_transformed

Dibuja un texto con espaciado, escala y ángulo personalizados.

## Síntaxis

  
```gml  
draw_text_ext_transformed(x, y, str, sep, w, xscale, yscale, angle);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal donde dibujar el texto.|  
y|La posición vertical donde dibujar el texto.|  
str|La cadena de texto a dibujar.|  
sep|La separación vertical entre líneas.|  
w|El anchor máximo del texto.|  
xscale|La escala horizontal del texto (1 es tamaño original).|  
yscale|La escala vertical del texto (1 es tamaño original).|  
angle|El ángulo del texto, en grados.|  

## Descripción

Esta función es una mezcla entre `draw_text_ext()` y `draw_text_transformed()`

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_halign(fa_center);  
draw_set_valign(fa_middle);  
image_angle += 1;  
draw_text_ext_transformed(room_width / 2, room_height / 2, keyboard_string, 10, 300, 2, 2, image_angle);  
```