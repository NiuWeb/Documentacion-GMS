# surface_get_height

Devuelve el alto en píxeles de una surface.

## Sintaxis

  
```gml  
surface_get_height(surface_id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a conocer su altura.|  

## Descripción

Esta función simplemente devuelve el alto, en píxeles, de la surface indicada.  
  
_**Nota:** Cuando se trabaja con surface existe la posibilidad que se destruyan en cualquier momento. Debe **siempre** comprobar si existen con `surface_exists()` antes de hacer algo con ellas._

## Devuelve

Número real

## Ejemplo

  
```gml  
sh = surface_get_height(surf);  
```  
El código anterior almacena el alto de la surface indexada en la variable "surf" dentro de la variable "sh".