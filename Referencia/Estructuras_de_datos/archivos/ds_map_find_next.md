

# ds_map_find_next

Busca y devuelve la siguiente llave del mapa dado, relativa a una llave dada.

## Síntaxis

  
```gml  
ds_map_find_next(id, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a usar.|  
key|La llave de la cual se buscará la siguiente.|  

## Descripción

Esta función devuelve la siguiente llave almacenada en el mapa, la cual se encuentra después de la llave especificada en la función. Esto es útil cuando quieres buscar en el mapa por un dato especifico, aunque debe evitarse en lo posible por ser potencialmente lento. Si no existe una llave siguiente la función devolverá `undefined`, por lo que debes de comprobar el valor devuelto con la función `is_undefined()`.

## Devuelve

Número real, Cadena de texto o Indefinido

## Ejemplo

  
```gml  
var size, key;  
size = ds_map_size(inventory);  
key = ds_map_find_first(inventory);  
for (var i = 0; i < size; i++;){  
    if key!= "gold"{  
        key= ds_map_find_next(inventory, key);  
    }  
    else{ break; }  
}  
```  
El código anterior crea variables temporales para guardar el tamaño y la primera llave almacenada por la computadora en el mapa dado. Luego usa un `for` para ver cada elemento, si el elemento actual no coincide con el buscado usa la función `ds_map_find_next()` para tomar la siguiente llave. Así hasta encontrar la llave "gold"; al hacerlo sale del `for`.