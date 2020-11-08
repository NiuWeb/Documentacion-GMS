# surface_get_width

Devuelve el ancho en píxeles de una surface.

## Sintaxis

  
```gml  
surface_get_width(surface_id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a conocer su ancho.|  

## Descripción

Esta función simplemente devuelve el ancho, en píxeles, de la surface indicada.  
  
_**Nota:** Cuando se trabaja con surface existe la posibilidad que se destruyan en cualquier momento. Debe **siempre** comprobar si existen con `surface_exists()` antes de hacer algo con ellas._

## Devuelve

Número real

## Ejemplo

  
```gml  
sw = surface_get_width(surf);  
```  
El código anterior almacena el ancho de la surface indexada en la variable "surf" dentro de la variable "sw".