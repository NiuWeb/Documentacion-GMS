

# ds_map_exists

Devuelve si la llave dad existe o no en el mapa(ds_map) dado.

## Síntaxis

  
```gml  
ds_map_exists(id, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El índice de la estructura de datos a comprobar.|  
key|La llave a comprobar.|  

## Descripción

Esta función devuelve `true` si la llave especificada existe en el mapa (previamente creado), y `false` si este no existe.

## Devuelve

Boleano

## Ejemplo

  
```gml  
if !ds_map_exists(inventory, "potions"){  
    ds_map_add(inventory, "potions", 1);  
}  
```  
El código anterior comprueba la mapa indexado en la variable "inventory", buscando la llave "potions" si esta no existe entonces la añade.