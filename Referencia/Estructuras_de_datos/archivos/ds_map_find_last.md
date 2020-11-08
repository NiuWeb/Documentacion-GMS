

# ds_map_find_last

Busca y devuelve la ultima llave, según el orden de almaceniento del PC, del mapa dado.

## Síntaxis

  
```gml  
ds_map_find_last(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a usar.|  

## Descripción

Esta función devuelve la ultima llave almacenada en el mapa. **¡Este orden no es el mismo en que has agregado las llaves!** Los mapas(ds_map) no almacenan la información de forma lineal, para ello usa listas(ds_list). Esto es útil cuando quieres buscar en todo el mapa por un dato especifico, aunque debe evitarse en lo posible por ser potencialmente lento.

## Devuelve

Número real o Cadena de texto

## Ejemplo

  
```gml  
var size = ds_map_size(inventory) ;  
var last = ds_map_find_first(inventory);  
for (var i = size; i > 0; i--;){  
    if last != "gold"{  
        last = ds_map_find_next(inventory, last);  
    }  
    else break;  
}  
```  
El código anterior crea variables temporales para guardar el tamaño y la ultima llave almacenada por la computadora en el mapa dado. Luego usa un `for` para ver cada elemento (desde el ultimo al primero) hasta encontrar la llave "gold"; al hacerlo sale del `for`.