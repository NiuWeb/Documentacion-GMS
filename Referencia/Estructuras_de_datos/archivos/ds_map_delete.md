

# ds_map_delete

Elimina la llave del mapa(ds_map) dado.

## Síntaxis

  
```gml  
ds_map_delete(id, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a modificar.|  
key|La llave (junto con su valor) a eliminar.|  

## Descripción

Esta función permite eliminar la llave dada (y también el valor asignado a dicha llave), en un mapa previamente creado.

## Devuelve

Nada

## Ejemplo

  
```gml  
ds_map_delete(inventory, "shield");  
```  
El código anterior elimina la llave "shield" (y su valor asignado) del mapa "inventory".