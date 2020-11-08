# filename_dir

Devuelve el directorio de un nombre de archivo.

## Sintaxis

  
```gml  
filename_dir(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre de archivo al cual obtener el directorio.|  

## Descripción

Esta función devuelve el directorio de un nombre de archivo dado. Normalmente equivale a la ruta del archivo sin la barra inclinada final.  
  
**NOTA:** Esta función no maneja archivos reales, sino que sólo trabaja con cadenas de texto, por lo que no importa si el archivo o ruta especificados no existen.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = "D:/Descargas/MyGame/Downloaded_Levels/level_137.dat";  
ext = filename_ext(file); //Devuelve '.dat'  
dir = filename_dir(file); //Devuelve 'D:/Descargas/MyGame/Downloaded_Levels'  
drive = filename_drive(file); //Devuelve 'D:'  
```