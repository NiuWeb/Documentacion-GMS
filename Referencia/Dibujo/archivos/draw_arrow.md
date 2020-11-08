# draw_arrow

Dibuja una flecha, la linea es de un pixel de ancho y es entre los puntos definidos por el usuario.

## Sintaxis

  
```gml  
draw_arrow(x1, y1, x2, y2, size);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La coordenada en x donde empezará la linea.|  
y1|La coordenada en y donde empezará la linea.|  
x2|La coordenada en x donde terminará la linea (incluyendo la punta de la flecha).|  
y2|La coordenada en y donde terminará la linea (incluyendo la punta de la flecha).|  
size|El largo de la punta de la flecha en pixeles.|  

## Descripción

Esta función dibuja una flecha desde el punto (x1, y1) al punto (x2, y2). La linea de la flecha se dibuja entre estos puntos incluyendo la punta de la flecha, por lo que el final de la punta de la flecha coincide con el punto (x2, y2). El tamaño de la punta de la flecha se define por el argumento `size` y el ancho de la punta de la flecha se calcula automáticamente en proporción a la longitud.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_arrow(x, y, mouse_x, mouse_y, 10);  
```  
El código anterior dibuja una flecha desde la posición de la instancia hasta la posición del ratón, con una punta de 10 píxeles de largo.