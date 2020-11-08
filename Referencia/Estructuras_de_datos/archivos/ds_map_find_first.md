

# ds_map_find_first

Busca y devuelve la primera llave, según el orden de almacenamiento del PC, del mapa dado.

## Síntaxis

  
```gml  
ds_map_find_first(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a usar.|  

## Descripción

Esta función devuelve la primera llave almacenada en el mapa. **¡Este orden no es el mismo en que has agregado las llaves!** Los mapas(ds_map) no almacenan la información de forma lineal, para ello usa listas(ds_list). Esto es útil cuando quieres buscar en todo el mapa por un dato especifico, aunque debe evitarse en lo posible por ser potencialmente lento.

## Devuelve

Número real o Cadena de texto

## Ejemplo

  
```gml  
var size = ds_map_size(inventory) ;  
var first = ds_map_find_first(inventory);  
for (var i = 0; i < size; i++;){  
    if first != "gold"{  
        first = ds_map_find_next(inventory, first);  
    }  
     else break;  
}  
```  
El código anterior crea variables temporales para guardar el tamaño y la primera llave almacenada por la computadora en el mapa dado. Luego usa un `for` para ver cada elemento hasta encontrar la llave "gold"; al hacerlo sale del `for`.