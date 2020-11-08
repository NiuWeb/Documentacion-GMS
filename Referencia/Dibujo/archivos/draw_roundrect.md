# draw_roundrect

Dibuja un rectángulo con los bordes redondeados.

## Síntaxis

  
```gml  
draw_roundrect(x1, y1, x2, y2, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La posición horizontal del primer punto del rectángulo a dibujar.|  
y1|La posición vertical del primer punto del rectángulo a dibujar.|  
x2|La posición horizontal del segundo punto del rectángulo a dibujar.|  
y2|La posición vertical del segundo punto del rectángulo a dibujar.|  
outline|¿Dibujar sólo el borde (true) del rectángulo, o el rectángulo relleno (false)?|  

## Descripción

Esta función permite dibujar un rectángulo con los bordes redondeados en el área definida por la ezquina superior izquierda (x1, y1) y la ezquina inferior derecha (x2, y2).  
  
Para definir la precisión de los bordes del rectángulo, use `draw_set_circle_precision()`.  
  
Sin embargo, esta función usa un radio fijo para los bordes. Si se desea utilizar un radio personalizado, use `draw_roundrect_ext()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_colour(c_lime);  
draw_roundrect(50, 100, 250, 200, false);  
```