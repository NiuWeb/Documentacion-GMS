# draw_text_colour

Dibuja un texto en la posición dada con espaciado y color personalizados.

## Síntaxis

  
```gml  
draw_text_ext_colour(x, y, string, sep, w, c1, c2, c3, c4, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal en donde dibujar el texto.|  
y|La posición vertical en donde dibujar el texto.|  
str|La cadena de texto a dibujar.|  
sep|La separación vertical entre líneas.|  
w|El anchor máximo de cada línea.|  
c1|El color de la ezquina superior izquierda del texto.|  
c2|El color de la ezquina superior derecha del texto.|  
c3|El color de la ezquina inferior derecha del texto.|  
c4|El color de la ezquina inferior izquierda del texto.|  
alpha|La opacidad del texto (1 es original).|  

## Descripción

Esta función es una mezcla entre `draw_text_ext()` y `draw_text_colour()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_colour(c_white);  
draw_text_ext_colour(200, 200, keyboard_string, 5, 300, c_blue, c_blue, c_navy, c_navy, 1);  
```