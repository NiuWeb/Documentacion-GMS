# script_get_name

Devuelve el nombre del script con el índice dado.

## Sintaxis

  
```gml  
script_get_name(scr);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
scr|El índice del _script_.|  

## Descripción

Esta función devuelve el nombre, como cadena de texto, del _script_ especificado. Este nombre es el que ha sido establecido para el _script_ en el árbol de recursos del IDE _Game Maker Studio_.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
nombre = script_get_name(scr_miScript);  
```  
Si el _script_ `scr_miScript` existe con el mismo nombre, la función devolverá `"scr_miScript"`.