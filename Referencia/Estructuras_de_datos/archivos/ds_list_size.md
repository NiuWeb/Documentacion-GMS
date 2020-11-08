# ds_list_size

Devuelve el número de valores almacenados dentro de la lista dada.

## Sintaxis

  
```gml  
ds_list_size(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a comprobar.|  

## Descripción

Esta función devuelve el "tamaño" de la lista, ejemplo: el número de elementos que han sido agregados a esta.

## Devuelve

Número real

## Ejemplo

  
```gml  
if !ds_list_empty(control_list){  
     num = ds_list_size(control_list);  
}  
```  
El código anterior comprueba si la lista esta vacía o no, si no esta vacía, obtiene el numero de elementos que contiene y almacena dicho dato dentro de una variable.