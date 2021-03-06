# draw_circle_colour

Dibuja un círculo del tamaño dado con un degradado circular de dos colores.

## Sintaxis

  
```gml  
draw_circle_colour(x, y, r, col1, col2, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La coordenada en x donde estará el centro del círculo|  
y|La coordenada en y donde estará el centro del círculo|  
r|El radio (distancia desde el centro al borde) del círculo en pixeles.|  
col1|El color del centro del círculo.|  
col2|El color del borde del círculo.|  
outline|Si el círculo se dibujará rellenado (false) o si se dibujará solo su contorno (true). Si es |  

## Descripción

Con esta función puede dibujar el contorno de un círculo o un círculo relleno. Si es un círculo lleno, puede definir dos colores, uno del interior y el otro del exterior. Si los colores dados no son los mismos, se hará un efecto de degradado, los argumentos de color tendrán prioridad sobre el color ajustado con la función `draw_set_colour()`. Se puede definir el grado de precisión del círculo con la función `draw_set_circle_precision()`.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_circle_colour(x, y, 100, c_white, c_black, false);  
```  
El código anterior dibuja un círculo relleno con su centro en la posición de la instancia que la ejecuta, con un radio de 100 píxeles, desde el color blanco en el centro hasta el color negro en el exterior.