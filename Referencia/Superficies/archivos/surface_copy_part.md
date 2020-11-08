# surface_copy_part

Copia parte de una surface dentro de otra surface (sin ningún tipo de blending).

## Sintaxis

  
```gml  
surface_copy_part(destination, x, y, source, xs, ys, ws, hs);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
destination|El ID de la surface en la que se copiará la otra surface.|  
x|La coordenada en x donde se copiará.|  
y|La coordenada en y donde se copiará.|  
source|El ID de la surface a copiar.|  
xs|La coordenada inicial en x de la surface que se copiará.|  
ys|La coordenada inicial en y de la surface que se copiará.|  
ws|El ancho del área que se desea copiar de la surface.|  
hs|El alto del área que se desea copiar de la surface.|  

## Descripción

Esta función simplemente toma lo dibujado en una surface y lo copia dentro de la surface especificada en el lugar que se le indique (donde la posición (0,0) es la esquina superior izquierda de la surface de destino). Puede especificar una posición "x" y "y" local de la surface a copiar, también el ancho y la altura del área. Tenga en cuenta que son coordenadas basadas en el tamaño de la surface y no en las coordenadas donde se dibuja la surface en el room (consulte la sección de Surfaces para mayor información). Si la surface de destino ya contiene información, esta será sobrescrita. La función no modifica la surface que se esta copiando.  
  
_**Nota:** Cuando se trabaja con surface, existe la posibilidad de que estas dejen de existir en cualquier momento, debido a que se almacenan en la memoria de texturas. Debe de **siempre** comprobar si existe la surface antes de usarlas con la función `surface_exists()` Para más información vea la sección de Surface._

## Devuelve

Nada

## Ejemplo

  
```gml  
if view_current == 0{  
     surface_copy_part(surf, 0, 0, 0, 0, view_xview[1] - mouse_x, view_yview[1] - mouse_y, temp_surf);  
}  
else{  
     draw_surface(surf, 0, 0);  
}  
```  
El código anterior comprobará la vista actual que se esta dibujando, si es la "view[0]", copia la surface indexada en la variable "temp_surf" sobre la surface indexada en la variable "surf". El área copiada corresponde a un rectángulo formando por la posición relativa del raton dentro del a surface tal como se dibujaría la view[1]. Si la vista actual es otra a la view[0], la surface "surf" se dibujara en pantalla.