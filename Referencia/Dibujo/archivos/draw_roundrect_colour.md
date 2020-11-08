# draw_roundrect_colour

Dibuja un rectángulo con bordes redondeados y una gradiente de dos colores.

## Síntaxis

  
```gml  
draw_roundrect_colour(x1, y1, x2, y2, col1, col2, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La posición horizontal del primer punto del rectángulo.|  
y1|La posición vertical del primer punto del rectángulo.|  
x2|La posición horizontal del segundo punto del rectángulo.|  
y2|La posición vertical del segundo punto del rectángulo.|  
col1|El color del centro de la gradiente del rectángulo.|  
col2|El color del margen de la gradiente del rectángulo.|  
outline|¿Dibujar sólo el borde del rectángulo (true), o el rectángulo relleno (false)?|  

## Descripción

Esta función permite dibujar un rectángulo con los bordes redondeados desde la ezquina superior izquierda (x1, y1) hasta la ezquina inferior derecha (x2, y2). Es posible escoger el color del centro y de los márgenes, los cuales se mezclaran dando un efecto degradado. Los colores definidos como parámetros tienen mayor prioridad que el color de dibujo actual, lo que significa que el color definido por `draw_set_colour()` será ignorado.  
  
Es posible definir la precisión de los bordes del rectángulo utilizando `draw_set_circle_precision()`. Sin embargo, las ezquinas tienen un radio fijo. Si se necesita personalizar el radio de los bordes, debe usarse `draw_roundrect_colour_ext()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_roundrect_colour(50, 50, 200, 200, c_black, c_white, false);  
```