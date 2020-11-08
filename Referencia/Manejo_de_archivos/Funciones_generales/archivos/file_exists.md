# file_exists

Comprueba si un archivo existe.

## Sintaxis

  
```gml  
file_exists(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El archivo a comprobar.|  

## Descripción

Esta función devolverá `true` si el archivo especificado existe, y `false` de lo contrario.

## Devuelve

Booleano

## Ejemplo

  
```gml  
if(file_exists("Completed_levels/level05.ini"))  
    show_message("¡Ya tienes una partida guardada en el nivel 5!");  
```