# surface_resize

Cambia el tamaño de una surface previamente creada.

## Sintaxis

  
```gml  
surface_resize(surface_id, w, h);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a modificar.|  
w|El nuevo ancho de la surface.|  
h|El nuevo alto de la surface.|  

## Descripción

Esta función cambiará el tamaño de una surface (en pixeles). El surface_id debe de ser una surface creada anteriormente, o la `application_surface`. Tenga en cuenta que esto no recortará ni estirará el contenido de la surface, si no que la destruirá y la volverá a crear con las nuevas dimensiones, lo que significa que tendrá que ser borrada y dibujada de nuevo (En el caso de la `application_surface` GameMaker: Studio se encargará de ello automáticamente).  
  
_**Nota:** Si esta cambiando el tamaño de la `application_surface`, estos cambios no se efectuarán hasta el inicio del siguiente cuadro (frame), lo que significa que si usa las funciones `surface_get_width()` o `surface_get_height()` en el mismo evento o step devolverá los valores anteriores._

## Devuelve

Nada

## Ejemplo

  
```gml  
if view_wport[0] != surface_get_width(application_surface) || view_hport[0] != surface_get_height(application_surface){  
     surface_resize(application_surface, view_wport[0],view_hport[0]);  
}  
```  
El código anterior comprueba si el tamaño del "port" de la vista es diferente del tamaño de la surface "application_surface" y si es diferente, la surface es re-dimensionada.