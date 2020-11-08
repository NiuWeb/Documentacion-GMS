# filename_name

Devuelve el nombre del archivo dado.

## Sintaxis

  
```gml  
filename_name(fname);  
```  

## Argumentos

Ninguno

## Descripción

Esta función obtiene la parte del nombre del nombre de archivo dado, con la extensión del mismo pero sin la ruta.  
  
  
NOTA: Esta función no hace uso de archivos reales, sólo maneja cadenas de texto; por lo que no importa si el archivo dado no existe.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = "D:/Descargas/MyGame/Downloaded_Levels/level_137.dat";  
name = filename_name(file); //Devuelve 'level_137.dat'  
ext = filename_ext(file); //Devuelve '.dat'  
dir = filename_dir(file); //Devuelve 'D:/Descargas/MyGame/Downloaded_Levels'  
drive = filename_drive(file); //Devuelve 'D:'  
```