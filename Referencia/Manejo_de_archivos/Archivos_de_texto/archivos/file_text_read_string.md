# file_text_read_string

Lee una cadena de texto del archivo de texto dado.

## Sintaxis

  
```gml  
file_text_read_string(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  

## Descripción

Esta función permite leer una cadena de texto del archivo de texto dado y devuelve el contenido leído como cadena de texto. Esta función sólo toma el contenido hasta el final de la línea (sin tomar el salto de línea) en la que se encuentra el puntero del archivo.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
lineas[0] = 0;  
pos = 0;  
file = file_text_open_read("datos.ini");  
while(!file_text_eof(file)) {  
    lineas[pos++] = file_text_read_string(file);  
    file_text_readln(file);  
}  
file_text_close(file);  
  
```  
El ejemplo anterior permite leer todas las líneas de un archivo de texto y guardarlas dentro de un _array_.