# draw_ellipse

Dibuja una elipse.

## Sintaxis

  
```gml  
draw_ellipse(x1, y1, x2, y2, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La coordenada en x del lado izquierdo de la elipse.|  
y1|La coordenada en y del lado superior de la elipse.|  
x2|La coordenada en x del lado derecho de la elipse.|  
y2|La coordenada en y del lado inferior de la elipse.|  
outline|Si la elipse se dibujará rellenado (false) o si se dibujará solo su contorno con un pixel de ancho (true).|  

## Descripción

Con esta función se puede dibujar el contorno de una elipse o una elipse rellenada, definida dentro de un área rectangular. Se puede definir la precisión de la elipse con la función `draw_set_circle_precision()`.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_ellipse(100, 100, 300, 200, false);  
```  
El código anterior dibuja una elipse dentro del área rectangular dada.