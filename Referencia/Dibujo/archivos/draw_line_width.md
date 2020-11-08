# draw_line_width

Dibuja una línea de un ancho definido.

## Sintaxis

  
```gml  
draw_line_width(x1, y1, x2, y2, w);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La coordenada en x donde comenzará la línea.|  
y1|La coordenada en y donde comenzará la línea.|  
x2|La coordenada en x donde terminará la línea.|  
y2|La coordenada en y donde terminará la línea.|  
w|El ancho de la linea, en pixeles.|  

## Descripción

Con esta función puedes dibujar una línea de un ancho especifico entre dos puntos definidos.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_line_width(100, 100, 200, 200, 6);  
```  
Con el código anterior se dibuja una línea diagonal de 6 pixeles de ancho, desde el punto (100, 100) hasta el punto (200, 200).