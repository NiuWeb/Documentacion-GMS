# draw_ellipse_colour

Dibuja una elipse con un degradado circular de dos colores.

## Sintaxis

  
```gml  
draw_ellipse_colour(x1, y1, x2, y2, col1, col2, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La coordenada en x del lado izquierdo de la elipse.|  
y1|La coordenada en y del lado superior de la elipse.|  
x2|La coordenada en x del lado derecho de la elipse.|  
y2|La coordenada en y del lado inferior de la elipse.|  
col1|El color del centro de la elipse.|  
col2|El color del borde de la elipse.|  
outline|Indica si dibuja el contorno de una elipse (true) o si es una elipse rellena (false).|  

## Descripción

Con esta función se puede dibujar el contorno de una elipse o una elipse rellena, definida dentro de un área rectangular dada. Si la elipse es rellena puede definir un color para el interior y otro para el borde. Si los colores no son iguales, se obtendra un efecto de degradado circular (los colores indicados reemplazan el color base indicado por la función `draw_set_colour()`). Puedes definir la precisión de la elipse con la función `draw_set_circle_precision()`.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_ellipse_colour(50, 50, 200, 100, c_black, c_white, false);  
```  
Con el código anterior se dibuja una elipse alargada horizontalmente, con un degradado desde el color negro(centro) y el color blanco(borde).