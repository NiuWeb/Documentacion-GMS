

# ds_map_destroy

Elimina el mapa dado de forma permanente, removiéndolo de la memoria.

## Síntaxis

  
```gml  
ds_map_destroy(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a eliminar|  

## Descripción

Los mapas toman un espacio en memoria, el cual es asignado cuando son creados. Por esta razón es necesario eliminarlos de la memoria cuando ya no es necesario, para prevenir errores, fugas de memoria o un lento rendimiento del juego. Esta función hace precisamente eso.

## Devuelve

Nada

## Ejemplo

  
```gml  
ds_map_destroy(inventory);  
```  
El código anterior elimina el mapa indexado en la variable "inventory".