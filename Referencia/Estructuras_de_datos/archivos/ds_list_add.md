# ds_list_add

Agrega el valor (o valores) dados al final de la lista.

## Sintaxis

  
```gml  
ds_list_add(id, val1, [val2, ... val15]);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a la que se agregaran.|  
val|El valor a agregar a la lista.|  
[val2, ... val15]|Valor opcionales a agregar a la lista.|  

## Descripción

Esta función puede ser usada para agregar un nuevo valor (número real o cadena de cadena de texto) a la lista, siempre serán agregados al final. Esta función puede tomar hasta 14 argumentos opcionales, permitiendo agregar múltiples valor de forma consecutiva a una lista desde una simple llamada.

## Devuelve

Nada

## Ejemplo

  
```gml  
ds_list_add(sc_list, score);  
```  
El código anterior agrega el valor almacenado en la variable "score" dentro de la lista indexada en la variable "sc_list".