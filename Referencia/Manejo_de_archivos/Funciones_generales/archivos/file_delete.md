# file_delete

Elimina el archivo especificado.

## Sintaxis

  
```gml  
file_delete(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El archivo a eliminar.|  

## Descripción

Esta función permite eliminar el archivo especificado del disco duro. Cabe mencionar que esta función sólo eliminará archivos que Game Maker Studio pueda crear y leer: archivos INI, archivos de texto y archivos binarios, o archivos creados para almacenar recursos del juego, como sprites o superficies. Esta función devuelve `true` si se ha podido eliminar el archivo, y `false` en cualquier caso de error.

## Devuelve

Booleano

## Ejemplo

  
```gml  
d = file_delete("Downloads/level03.ini");  
if(d)  
    show_message("El nivel descargado ha sido eliminado con éxito");  
```