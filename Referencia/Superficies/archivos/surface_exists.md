# surface_exists

Devuelve si en la variable dada existe una surface.

## Sintaxis

  
```gml  
surface_exists(surface_id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a comprobar.|  

## Descripción

Esta función es esencial al momento de trabajar con surface por la naturaleza volátil de estas. Las superficies siempre se mantienen en la memoria de textura, lo que significa que pueden destruirse de un momento a otro (por ejemplo, cuando se inicia el protector de pantalla en Windows o cuando se minimiza en un dispositivos Android), por lo que siempre debe de comprobar si existe la surface antes de trabajar con ellas (incluyendo el dibujarlas en pantalla). El código de ejemplo muestra un uso típico de este comando en el evento draw de una instancia, donde comprueba la surface y vuelve a crearla si se ha eliminado (tenga en cuenta que la surface se creo originalmente en el evento create del objeto).

## Devuelve

Boleano

## Ejemplo

  
```gml  
if !surface_exists(surf){  
     surf = surface_create(1024, 1024);  
}  
else{  
     if view_current = 1{  
          draw_surface(surf,0,0);  
     }  
}  
```  
El código anterior comprueba si existe una surface indexada en la variable "surf", si no es así, entonces la vuelve a crear. Si existe, entonces comprueba cual es la vista actual que se esta dibujando, si es la view[1] entonces dibujará la surface.