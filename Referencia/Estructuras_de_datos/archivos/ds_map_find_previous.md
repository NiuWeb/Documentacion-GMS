

# ds_map_find_previous

Busca y devuelve la llave anterior del mapa dado, relativa a una llave dada.

## Síntaxis

  
```gml  
ds_map_find_previous(id, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a usar.|  
key|La llave de la cual se buscará la anterior.|  

## Descripción

Esta función devuelve la llave anterior almacenada en el mapa, la cual se encuentra antes de la llave especificada en la función. Esto es útil cuando quieres buscar en el mapa por un dato especifico, aunque debe evitarse en lo posible por ser potencialmente lento. Si no existe una llave anterior función devolverá `undefined`, por lo que debes de comprobar el valor devuelto con la función `is_undefined()`.

## Devuelve

Número real, Cadena de texto o Indefinido

## Ejemplo

  
```gml  
var size, key;  
size = ds_map_size(inventory);  
key = ds_map_find_last(inventory);  
for (var i = size; i > 0; i--;){  
    if key!= "gold"{  
        key= ds_map_find_previous(inventory, key);  
    }  
     else{ break; }  
}  
```  
El código anterior crea variables temporales para guardar el tamaño y la ultima llave almacenada por la computadora en el mapa dado. Luego usa un `for` para ver cada elemento, si el elemento actual no coincide con el buscado usa la función `ds_map_find_previous()` para tomar la llave anterior. Así hasta encontrar la llave "gold"; al hacerlo sale del `for`.