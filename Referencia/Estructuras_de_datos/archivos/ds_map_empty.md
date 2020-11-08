

# ds_map_empty

Devuelve si el mapa dado esta vacío o no.

## Síntaxis

  
```gml  
ds_map_empty(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a comprobar.|  

## Descripción

Esta función devuelve `false` si el mapa dado contiene algún par de llave-valor, devuelve `true` en caso contrario.

## Devuelve

Boleano

## Ejemplo

  
```gml  
if ds_map_empty(inventory){  
weight = 0;  
}  
```  
El código anterior comprueba si el mapa indexado en la variable "inventory" contiene algún par de llave-valor y si este no contiene ninguno, "weight" será 0.