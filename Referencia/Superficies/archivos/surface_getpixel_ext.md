# surface_getpixel_ext

Devuelve el valor completo en 32bit del pixel en las coordenadas dadas de una surface.

## Sintaxis

  
```gml  
surface_getpixel_ext(surface_id, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface.|  
x|La posición en x, de la surface, de donde se tomará el pixel.|  
y|La posición en y, de la surface, de donde se tomará el pixel.|  

## Descripción

Con esta función se obtiene el valor completo de **abgr en 32bit** de cualquier pixel de una surface(previamente creada).  
  
_**Nota:** Esta función es lenta y solo debe ser usada cuando es absolutamente necesaria._

## Devuelve

Número real

## Ejemplo

  
```gml  
col = surface_getpixel_ext(mouse_x, mouse_y);  
alpha = (col >> 24) & 255;  
blue = (col >> 16) & 255;  
green = (col >> 8) & 255;  
red = col & 255;  
```  
El código anterior obtiene el valor del color en 32bits de la posición del ratón y luego lo separa en sus valores que lo compone para almacenarlos en variables.