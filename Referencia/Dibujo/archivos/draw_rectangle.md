# draw_rectangle

Dibuja un rectángulo.

## Sintaxis

  
```gml  
draw_rectangle(x1, y1, x2, y2, outline);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La coordenada en x del lado izquierdo del rectángulo.|  
y1|La coordenada en y del lado superior del rectángulo.|  
x2|La coordenada en x del lado derecho del rectángulo.|  
y2|La coordenada en y del lado abajo del rectángulo.|  
outline|Indica si el rectangulo se dibujará relleno(false) o si se dibujará con un contorno de un pixel(true).|  

## Descripción

Con esta función puede dibujar el contorno de un rectángulo o un rectángulo relleno, desde el punto (x1, y1) el cual corresponde a la esquina superior izquierda y el punto (x2, y2) el cual corresponde a la esquina inferior derecha.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_rectangle(100, 100, 300, 200, true);  
```  
Con el código anterior se dibuja el contorno de un rectángulo, con su esquina superior izquierda en el punto (100, 100) y su esquina inferior derecha en el punto (300, 200).