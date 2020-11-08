# draw_line_colour

Dibuja una línea con una gradiente de color.

## Síntaxis

  
```gml  
draw_line_colour(x1, y1, x2, y2, col, col2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La posición horizontal del primer punto de la línea.|  
y1|La posición vertical del primer punto de la línea.|  
x2|La posición horizontal del segundo punto de la línea.|  
y2|La posición vertical del segundo punto de la línea.|  
col1|El primer color de la línea.|  
col2|El segundo color de la línea.|  

## Descripción

Esta función dibuja una línea de 1px de grosor desde el punto (x1, y1) hasta (x2, y2) con un color que se degrada desde col1 hasta col2. El color definido por `draw_set_colour()` es ignorado.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_line_colour(50, 50, 300, 50, c_red, c_blue);  
```  
Se dibuja una línea desde (50,50) hasta (300, 500), degradándose de rojo a azul.