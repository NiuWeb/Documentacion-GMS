# draw_triangle

Dibuja un triángulo mediante tres puntos dados.

## Síntaxis

  
```gml  
draw_triangle(x1, y1, x2, y2, x3, y3, outline);  
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
outline|¿Dibujar sólo el borde del triángulo (true), o el triángulo relleno (false)?|  

## Descripción

Esta función permite dibujar un triángulo definido por los tres puntos (x1, y1), (x2, y2) y (x3, y3).

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_colour(c_aqua);  
draw_triangle(50, 50, 200, 50, 50, 200, 0);  
```