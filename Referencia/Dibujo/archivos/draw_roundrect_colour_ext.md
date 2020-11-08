# draw_roundrect_colour_ext

Dibuja un rectángulo con un color y radio personalizados.

## Síntaxis

  
```gml  
draw_roundrect_colour_ext(x1, y1, x2, y2, xrad, yrad, col1, col2, outline);  
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
col1|El color del centro del rectángulo.|  
col2|El color del margen del rectángulo.|  
outline|¿Dibujar sólo el borde del rectángulo (true), o el rectángulo relleno (false)?|  

## Descripción

Esta función es una mezcla entre `draw_roundrect_ext()` y `draw_roundrect_colour()`.  
  
Para modificar la precisión de los bordes, use `draw_set_circle_precision()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_roundrect_colour_ext(x - 50, y - 50, x + 50, y + 50, 8, 8, c_red, c_white, 0);  
```