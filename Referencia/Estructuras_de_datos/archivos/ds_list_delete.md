# ds_list_delete

Elimina el valor de la posición dada de la lista.

## Sintaxis

  
```gml  
ds_list_delete(id, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a modificar.|  
pos|Posición donde está el valor a eliminar.|  

## Descripción

Con esta función puede eliminar el valor almacenado en una posición en especifico dentro de la lista.

## Devuelve

Nada

## Ejemplo

  
```gml  
if ds_list_size(sc_list) > 10{  
     while (ds_list_size(sc_list) > 10){  
          ds_list_delete(sc_list, 0);  
     }  
}  
```  
El código anterior comprueba el tamaño de la lista, si es mayor a diez, entra en un bucle que remueve consecutivamente el valor de la posición 0 hasta que la lista tenga solo 10 valores.