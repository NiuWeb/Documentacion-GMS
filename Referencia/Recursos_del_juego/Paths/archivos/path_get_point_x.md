# path_get_point_x

Devuelve la coordenada x del punto especificado del path dado.

## Sintaxis

  
```gml  
path_get_point_x(index, n);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  
n|El número del punto a comprobar.|  

## Descripción

Esta función devuelve la posición en X (de las coordenadas del room) del punto dado del path. Si el punto a comprobar está fuera del rango del path (ejemplo, si el path tiene 8 puntos y se pide la posición en X del punto 10) devolverá 0.

## Devuelve

Número real

## Ejemplo

  
```gml  
if path_position = 1{  
     var i;  
     i = floor(random(path_get_number(mypath)));  
     x = path_get_point_x(mypath, i);  
     y = path_get_point_y(mypath, i);  
     path_position = (1 / path_get_number(mypath)) * i;  
}  
```  
El código anterior comprueba si una instancia esta al final del path. Si es cierto, elegirá un punto aleatorio del path y moverá a la instancia a ese punto.