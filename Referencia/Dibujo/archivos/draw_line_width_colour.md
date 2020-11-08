# draw_line_width_colour

Dibuja una lína con un color y grosor determinados.

## Síntaxis

  
```gml  
draw_line_width_colour(x1, y1, x2, y2, w, col1, col2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La posición horizontal del primer punto de la línea.|  
y1|La posición vertical del primer punto de la línea.|  
x2|La posición horizontal del segundo punto de la línea.|  
y2|La posición vertical del segundo punto de la línea.|  
w|El grosor en pixeles de la línea.|  
col1|El primer color de la línea.|  
col2|El segundo color de la línea.|  

## Descripción

Esta función es una mezcla entre `draw_line_width()` y `draw_line_colour()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_line_width_colour(50, 50, 300, 50, 4, c_red, c_blue);  
```