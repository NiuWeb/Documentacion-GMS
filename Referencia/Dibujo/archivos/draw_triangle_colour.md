# draw_triangle_colour

Dibuja un triángulo mediante tres puntos dados con un color personalizado.

## Síntaxis

  
```gml  
draw_triangle_colour(x1, y1, x2, y2, x3, y3, col1, col2, col3, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La posición horizontal del primer punto del triángulo|  
y1|La posición vertical del primer punto del triángulo|  
x2|La posición horizontal del segundo punto del triángulo|  
y2|La posición vertical del segundo punto del triángulo|  
x3|La posición horizontal del tercer punto del triángulo|  
y3|La posición verticaldel tercer punto del triángulo|  
col1|El color de la primera ezquina del triángulo.|  
col2|El color de la segunda ezquina del triángulo.|  
col3|El color de la tercera ezquina del triángulo.|  
outline|¿Dibujar sólo el borde del triángulo (true), o el triángulo relleno (false)?|  

## Descripción

Esta función permite dibujar un triángulo definido por los tres puntos (x1, y1), (x2, y2) y (x3, y3) con los tres colores dados que se mezclan en una gradiente. Los colores definidos como parámetro se sobreponen al color definido por `draw_set_colour()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_triangle_colour(200, 200, 300, 200, 200, 300, c_red, c_green, c_blue, false);  
```