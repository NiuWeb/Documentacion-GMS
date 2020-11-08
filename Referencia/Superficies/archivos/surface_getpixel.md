# surface_getpixel

Devuelve el color de una pixel correspondiente a una posición de la surface.

## Sintaxis

  
```gml  
surface_getpixel(surface_id, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface.|  
x|La posición en x, de la surface, de donde se tomará el pixel.|  
y|La posición en y, de la surface, de donde se tomará el pixel.|  

## Descripción

Esta función puede ser usada para obtener el color de un pixel en especifico, de una surface; usando las coordenadas locales del a surface donde (0, 0) es la esquina superior izquierda. Esta función es extremadamente lenta y puede causar una pausa en el juego.  
  
_**Nota:** Cuando se trabaja con surface existe la posibilidad que se destruyan en cualquier momento. Debe **siempre** comprobar si existen con `surface_exists()` antes de hacer algo con ellas._

## Devuelve

Número real

## Ejemplo

  
```gml  
col = surface_getpixel(surf, 56, 78 );  
```  
El código anterior devuelve el color del pixel en las coordenadas (56, 78) de la surface indexada en la variable "surf".