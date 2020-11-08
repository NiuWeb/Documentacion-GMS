# point_distance_3d

Obtiene la distancia en pixeles entre dos puntos ubicados en un espacio tridimensional.

## Sintaxis

  
```gml  
point_distance_3d(x1, y1,  z1, x2, y2, z2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|La componente x del primer punto.|  
y1|La componente y del primer punto.|  
z1|La componente z del primer punto.|  
x2|La componente x del segundo punto.|  
y2|La componente y del segundo punto.|  
z2|La componente z del segundo punto.|  

## Descripción

Esta función devuelve la distancia entre un punto (x1, y1, z1) y otro (x2, y2, z2). Esta función trabaja prácticamente igual a `point_distance()`, con la excepción de que usa la coordenada z, para espacios tridimensionales.

## Devuelve

Número real.

## Ejemplo

  
```gml  
var distancia = point_distance_3d(x, y, posz, enemigo.posx, enemigo.posy, enemigo.posz);  
  
```  
Se obtiene la distancia y la dirección que hay entre el objeto actual y el objeto _enemigo_, asumiendo que se trata de un espacio tridimensional.