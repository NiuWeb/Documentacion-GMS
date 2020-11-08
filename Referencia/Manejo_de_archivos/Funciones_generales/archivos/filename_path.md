# filename_path

Devuelve la ruta de un nombre de archivo.

## Sintaxis

  
```gml  
filename_path(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre de archivo al cual obtener la ruta.|  

## Descripción

Esta función devuelve la ruta de un nombre de archivo dado **con** la barra inclinada final.  
  
**NOTA:** Esta función no maneja archivos reales, sino que sólo trabaja con cadenas de texto, por lo que no importa si el archivo o ruta especificados no existen.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = "D:/Descargas/MyGame/Downloaded_Levels/level_137.dat";  
name = filename_name(file); //Devuelve 'level_137.dat'  
dir = filename_path(file); //Devuelve 'D:/Descargas/MyGame/Downloaded_Levels'  
drive = filename_drive(file); //Devuelve 'D:'  
```