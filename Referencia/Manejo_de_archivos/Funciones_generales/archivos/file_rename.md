# file_rename

Renombra el archivo dado.

## Sintaxis

  
```gml  
file_rename(fname, newname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El archivo a renombrar|  
newname|El nuevo nombre del archivo.|  

## Descripción

Esta función permite renombrar el archivo especificado por el nuevo nombre dado. La función devuelve `true` si el archivo se ha renombrado exitosamente, o `false` en caso contrario.

## Devuelve

Booleano

## Ejemplo

  
```gml  
if(file_exists("Downloads/level_03.ini"))  
    file_rename("Downloads/level_03.ini", "Downloads/level_03_Completed.ini");  
```  
Si el archivo `"level_03.ini"` existe dentro del directorio `"Downloads"`, renombrarlo por `"level_03_Completed.ini"`.