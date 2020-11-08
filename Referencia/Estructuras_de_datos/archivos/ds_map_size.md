

# ds_map_size

Devuelve el tamaño del mapa dado.

## Síntaxis

  
```gml  
ds_map_size(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a comprobar.|  

## Descripción

Esta función le permite conocer cuantos pares de llaves-valores se encuentran en el mapa (previamente creado) dado.

## Devuelve

Número real

## Ejemplo

  
```gml  
if ds_map_size(inventory) > 49{  
    full = true;  
}  
```  
El código anterior comprueba si el tamaño del mapa indexado en la variable "inventory" es mayor a 49, si es cierto, la variable "full" será `true`.