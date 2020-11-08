# ds_list_find_value

Busca el valor de la posición dada dentro de la lista.

## Sintaxis

  
```gml  
ds_list_find_value(id, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a usar.|  
pos|La posición a comprobar, donde 0 corresponde al inicio de la lista y la posición final sería ds_list_size(id)-1.|  

## Descripción

Con esta función puede comprobar dentro de la lista la posición dada y obtener su valor almacenado.  
  
_**Nota:** Si da una posición fuera del tamaño de la lista (ejemplo, la posición 11 en una lista de 10 valores), la función devolverá <Indefinido(undefined)>. Siempre se debe comprobar lo obtenido con la función `is_undefined()`_

## Devuelve

Número real, Cadena de texto o Indefinido.

## Ejemplo

  
```gml  
val = ds_list_find_value(list, ds_list_size(list) - 1);  
```  
El código anterior comprobará en la lista indexada en la variable "list", la ultima posición y almacenará el valor devuelto dentro de la variable "val".