# draw_circle

Dibuja un circulo.

## Sintaxis

  
```gml  
draw_circle(x, y, r, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La coordenada en x donde estará el centro del círculo|  
y|La coordenada en y donde estará el centro del círculo|  
r|Radio del círculo (la longitud desde el centro hasta su borde).|  
outline|Si el círculo se dibujará rellenado (false) o si se dibujará solo su contorno (true).|  

## Descripción

Con esta función se puede dibujar el contorno de un círculo o bien un círculo relleno. Puede definir la precisión del dibujo con la función `draw_set_circle_precision()`.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_circle(100, 100, 50, true);  
```  
El codigo anterior dibuja el contorno de un círculo con un radio de 50 pixeles.