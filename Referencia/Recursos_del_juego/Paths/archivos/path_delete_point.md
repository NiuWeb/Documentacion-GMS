# path_delete_point

Elimina un punto existente del path dado.

## Sintaxis

  
```gml  
path_delete_point(index, n);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path que contiene el punto a eliminar.|  
n|El número del punto a eliminar.|  

## Descripción

Con esta función puede eliminar un punto del path especificado. Los puntos del path son enumerados desde el 0, por lo que el punto 0 siempre sera el primero y el último punto del path siempre será `path_get_number() - 1`.

## Devuelve

Nada

## Ejemplo

  
```gml  
path_delete_point(mypath, path_number(mypath) - 1);  
```  
El código anterior elimina el ultimo punto del path indexado en la variable "mypath".