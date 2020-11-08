# directory_exists

Comprueba si un directorio existe o no.

## Sintaxis

  
```gml  
directory_exists(dname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
dname|El nombre del directorio a examinar.|  

## Descripción

Esta función comprueba si el directorio indicado existe (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano

## Ejemplo

  
```gml  
if(directory_exists("Game/DLC_v1"))  
    show_message("Ya has descargado el DLC anteriormente");  
```