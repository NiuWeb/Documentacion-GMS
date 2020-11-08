# directory_destroy

Elimina el directorio con el nombre dado.

## Sintaxis

  
```gml  
directory_destroy(dname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
dname|El nombre del directorio a eliminar.|  

## Descripción

Elimina el directorio especificado del área de guardado local (_sandbox_).

## Devuelve

Nada

## Ejemplo

  
```gml  
if(directory_exists("Game/Comments"))  
    directory_destroy("Game/Comments");  
```  
Si el directorio **Comments**, ubicado en el directorio **Game** del área de guardado local (_sandbox_), existe, entonces eliminarlo.