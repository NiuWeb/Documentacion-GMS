# surface_create

Crea una surface.

## Sintaxis

  
```gml  
surface_create(w, h);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
w|El ancho de la surface a crear.|  
h|El alto de la surface a crear.|  

## Descripción

Esta función es usada para crear una surface, se devolverá el índice de la surface, que debe de ser almacenada en una variable, para ser usada con otras funciones. Cuando la surface se crea, puede contener "ruido" ya que es una área de memoria que se reserva (y esa memoria puede contener información anterior), por lo que es recomendado limpiar la surface con una función como `draw_clear_alpha()`.  
  
Es muy recomendado que todas las surfaces creadas tengan un tamaño que sea potencia de 2, ejemplo: 16, 128, 512 o 1024 pixeles. Esto no es absolutamente necesario en ciertas plataformas (como Windows y MacOS) pero incrementa la compatibilidad en esas plataformas, mientras que en HTML5 y algunos dispositivos es esencial, por lo que es importante prestar atención para evitar problemas futuros.

## Devuelve

Número real

## Ejemplo

  
```gml  
if !surface_exists(surf){  
     surf = surface_create(1024, 1024);  
     surface_set_target(surf);  
     draw_clear_alpha(c_black, 0);  
     surface_reset_target();  
     view_surface_id[0] = surf;  
}  
```  
El código anterior comprueba si existe una surface, de no existir la creará con un tamaño de 1024 píxeles de ancho y alto, almacenando su índice en la variable "surf". El objetivo de dibujado es cambiado a la surface recién creada para borrar todo su contenido, luego se restablece el objetivo de dibujado. Finalmente la superficie es asignada a una view.