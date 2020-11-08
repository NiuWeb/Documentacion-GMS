# path_clear_points

Elimina todos los puntos del path dado.

## Sintaxis

  
```gml  
path_clear_points(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a limpiar.|  

## Descripción

Con esta función puede remover todos los puntos definidos en el path, siendo este ahora un path "vació". Esto _no_ elimina el path, para ello debe usar `path_delete`.

## Devuelve

Nada

## Ejemplo

  
```gml  
if path_get_number(mypath) > 0{  
     path_clear_points(mypath);  
}  
```  
El código anterior comprueba si el path "mypath" posee al menos 1 punto, si es cierto, limpia el path.