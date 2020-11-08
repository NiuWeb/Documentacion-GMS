# ds_list_find_index

Busca la posición del valor dado dentro de la lista.

## Sintaxis

  
```gml  
ds_list_find_index(id, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a usar.|  
val|El valor a buscar.|  

## Descripción

Con esta función puede comprobar la lista dada, que devolverá la posición del valor dado dentro de dicha lista. Tenga en cuenta que si hay más de una entrada con el mismo valor, la posición de cualquiera de los dos puede ser devuelta, y si el valor no existe devolverá `-1`.  
  
_**Nota:** Si el índice que deseas buscar en la lista es un arreglo (array), esta función devolverá `-1`_.

## Devuelve

Número real

## Ejemplo

  
```gml  
pos = ds_list_find_index(list, "Player1");  
```  
El código anterior buscará dentro la lista indexada en la variable "list" la posición del valor "Player1" y lo almacenará dentro de la variable "pos".