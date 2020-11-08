# point_distance

Obtiene la distancia en pixeles entre un punto y otro.

## Sintaxis

  
```gml  
point_distance(x1, y1, x2, y2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La componente horizontal del primer punto.|  
y1|La componente vertical del primer punto.|  
x2|La componente horizontal del segundo punto.|  
y2|La componente vertical del segundo punto.|  

## Descripción

Esta función devuelve la distancia entre un punto (x1, y1) y otro (x2, y2).

## Devuelve

Número real.

## Ejemplo

  
```gml  
var distancia = point_distance(x, y, enemigo.x, enemigo.y);  
var angulo    = point_direction(x, y, enemigo.x, enemigo.y);  
var tiempo    = room_speed;  
  
direction = angulo;  
speed     = distancia / tiempo;  
  
```  
Se obtiene la distancia y la dirección que hay entre el objeto actual y el objeto _enemigo_, y posteriormente se asigna a la variable `speed` el valor necesario para recorrer dicha distancia en un segundo.