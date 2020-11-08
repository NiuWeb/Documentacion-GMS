# filename_drive

Devuelve el disco en donde se almacena el nombre archivo dado.

## Sintaxis

  
```gml  
filename_drive(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre de archivo a obtener el disco.|  

## Descripción

Esta función permite obtener el disco de una ruta dada.  
  
**NOTA:** Esta función no maneja archivos reales, sino que solamente trabaja con cadenas de texto, por lo que no importa si la ruta o nombre de archivo especificados no existen.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = "D:/Descargas/MyGame/Downloaded_Levels/level_137.dat";  
ext = filename_ext(file); //Devuelve '.dat'  
dir = filename_dir(file); //Devuelve 'D:/Descargas/MyGame/Downloaded_Levels'  
drive = filename_drive(file); //Devuelve 'D:'  
```