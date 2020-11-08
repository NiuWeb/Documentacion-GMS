# filename_ext

Obtiene la extensión de un nombre de archivo.

## Sintaxis

  
```gml  
filename_ext(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre de archivo al cual obtener la extensión.|  

## Descripción

Esta función devuelve la parte de la extensión del nombre de un archivo, incluyendo el punto.  
  
**NOTA:** Esta función no maneja archivos reales, sólo trabaja con cadenas de texto, por lo que no importa si el nombre de archivo ingresado no existe.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = "D:/Descargas/MyGame/Downloaded_Levels/level_137.dat";  
ext = filename_ext(file); //Devuelve '.dat'  
dir = filename_dir(file); //Devuelve 'D:/Descargas/MyGame/Downloaded_Levels'  
drive = filename_drive(file); //Devuelve 'D:'  
```