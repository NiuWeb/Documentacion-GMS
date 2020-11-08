# ds_list_replace

Reemplaza el valor de cualquier posición dentro de la lista dada.

## Sintaxis

  
```gml  
ds_list_replace(id, pos, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a modificar.|  
pos|La posición donde se reemplazará el valor, donde 0 correspondo al inicio de la lista y el final sería ds_list_size(id)-1.|  
val|El nuevo valor que será puesto dentro de la lista.|  

## Descripción

Esta función puede remplazar el valor que se encuentra dentro de la posición dada de la lista, por uno nuevo.

## Devuelve

Nada

## Ejemplo

  
```gml  
ds_list_replace(n_list, 3, name);  
```  
EL código anterior reemplaza el valor almacenado en la posición 3 dentro de la lista por el valor almacenado en la variable "name".