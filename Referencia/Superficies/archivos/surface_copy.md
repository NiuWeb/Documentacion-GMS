# surface_copy

Copia el contenido de una surface dentro de otra surface.

## Sintaxis

  
```gml  
surface_copy(destination, x, y, source);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
destination|El ID de la surface en la que se copiará la otra surface.|  
x|La coordenada en x donde se copiará.|  
y|La coordenada en y donde se copiará.|  
source|El ID de la surface a copiar.|  

## Descripción

Esta función simplemente toma lo dibujado en una surface y lo copia dentro de la surface especificada en el lugar que se le indica (donde la posición (0,0) es la esquina superior izquierda de la surface de destino). Si la surface de destino tiene información, será sobrescrita por la información que se esta copiando, esta función no modificará la surface que se esta copiando.  
  
_**Nota:**Cuando se trabaja con surface, existe la posibilidad de que estas dejen de existir en cualquier momento, debido a que se almacenan en la memoria de texturas. Debe de **siempre** comprobar si existe la surface antes de usarlas con la función `surface_exists()` Para más información vea la sección de Surface_.

## Devuelve

Nada

## Ejemplo

  
```gml  
if view_current == 0{  
     surface_copy(surf, 0, 0, temp_surf);  
}  
else{  
     draw_surface(surf, 0, 0);  
}  
```  
El código anterior comprueba si la vista actual que esta siendo dibujada, si es la "view[0]", copia la surface indexada en la variable "temp_surf" sobre la surface indexada en la variable "surf". Si la vista actual es cualquier otra a "view[0]", la surface "surf" se dibujará en pantalla.