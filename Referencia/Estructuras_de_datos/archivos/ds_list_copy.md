# ds_list_copy

Copia una lista dentro de otra.

## Sintaxis

  
```gml  
ds_list_copy(id, source);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista en la que se copiará.|  
source|El id de la lista que será copiada.|  

## Descripción

Con esta función puede copiar el contenido de una lista dentro de otra. Las listas deben de ser creadas anteriormente y si la lista en la que se copiará contiene información, esa información será eliminada primero. El resultado son dos listas independientes que contienen la misma información.

## Devuelve

Nada

## Ejemplo

  
```gml  
if !ds_list_empty(main_list){  
     old_list = ds_list_create();  
     ds_list_copy(old_list, main_list);  
     ds_list_clear(main_list);  
}  
```  
El código anterior comprueba una lista para saber si está vacía. Si no está vacía, se copia su información en otra lista (se se creo anteriormente) y por último se limpia la lista original.