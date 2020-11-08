# ds_list_insert

Inserta el valor dado en cualquier posición dentro de la lista.

## Sintaxis

  
```gml  
ds_list_insert(id, pos, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista en que se añadirá.|  
pos|La posición del valor a agregar, donde 0 corresponde al comienzo de la lista y el final sería ds_list_size(id)-1.|  
val|EL valor a agregar a la lista.|  

## Descripción

Esta función agregará el valor dado en la lista en la posición dada. Si la lista contiene valores después de la posición dada, se desplazarán todos los valores para hacer espacio al nuevo valor, por lo que la lista aumentará su tamaño en 1.

## Devuelve

Nada

## Ejemplo

  
```gml  
ds_list_insert(list, 9, score);  
```  
El código anterior agregara el valor almacenado dentro de la variable "score" dentro de la posición 10 de la lista indexada en la variable "list" (las listas empiezan a contabilizarse desde el 0, una lista de 10 valores esta numerada desde el 0 hasta el 9).