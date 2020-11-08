# ds_list_sort

Ordena los valores de una lista según el tamaño, de forma ascendente o descendente.

## Sintaxis

  
```gml  
ds_list_sort(id, ascend);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a ordenar.|  
ascend|Si los valores serán ordenados de forma ascendente (true) o descendente (false).|  

## Descripción

Con esta función puede ordenar todos los valores dentro de una lista, en orden ascendente o descendente. Si la lista contiene cadenas de texto, entonces se ordenarán alfabéticamente, basados en las 26 letras del alfabeto inglés.

## Devuelve

Nada

## Ejemplo

  
```gml  
if newgame{  
     ds_list_sort(name_list, true);  
}  
```  
El código anterior ordena la lista indexada en la variable "name_list" si la variable "newgame" está marcada como `true`.