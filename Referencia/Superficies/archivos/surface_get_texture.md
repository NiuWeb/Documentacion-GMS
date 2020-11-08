# surface_get_texture

Devuelve el id de la textura de la surface dada.

## Sintaxis

  
```gml  
surface_get_texture(surface_id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a obtener su textura.|  

## Descripción

Esta función devuelve un _indicador_ especial textura de la surface. Este valor puede ser usado en otras funciones de dibujo, generalmente usado en 3D y algunas funciones 2D de primitivas.  
  
_**Nota:** Cuando se trabaja con surface existe la posibilidad que se destruyan en cualquier momento. Debe **siempre** comprobar si existen con `surface_exists()` antes de hacer algo con ellas._

## Devuelve

Indicador

## Ejemplo

  
```gml  
var tex;  
tex = surface_get_texture(surf);  
draw_primitive_begin_texture(pr_trianglestrip, tex);  
draw_vertex_texture(0, 480, 0, 0);  
draw_vertex_texture(640, 480, 1, 0);  
draw_vertex_texture(640, 480, 1, 1);  
draw_vertex_texture(0, 480, 0, 1);  
draw_primitive_end();  
```  
El código anterior dibuja 4 vértices de una tira de triángulos con textura, el indicador de la textura esta en la variable "tex", que fue tomada de la surface creada con anterioridad.