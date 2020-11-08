# draw_roundrect_ext

Dibuja un rectángulo con bordes redondeados de un radio personalizado.

## Síntaxis

  
```gml  
draw_roundrect_ext(x1, y1, x2, y2, xrad, yrad, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La posición horizontal del primer punto del rectángulo.|  
y1|La posición vertical del primer punto del rectángulo.|  
x2|La posición horizontal del segundo punto del rectángulo.|  
y2|La posición vertical del segundo punto del rectángulo.|  
xrad|El radio horizontal de los bordes.|  
yrad|El radio vertical de los bordes.|  
outline|¿Dibujar sólo el borde del rectángulo (true), o el rectángulo relleno (false)?|  

## Descripción

Esta función permite dibujar un rectángulo con los bordes redondeados desde la ezquina superior izquierda (x1, y1) hasta la ezquina inferior derecha (x2, y2). Es posible establecer el radio de los bordes de este rectángulo.  
  
Para modificar la precisión de los bordes, use `draw_set_circle_precision()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_roundrect_ext(x - 50, y - 50, x + 50, y + 50, 8, 8, false);  
```