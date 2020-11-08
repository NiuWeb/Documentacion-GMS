# file_text_readln

Mueve el puntero de un archivo de texto hasta la siguiente línea.

## Sintaxis

  
```gml  
file_text_readln(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  

## Descripción

Esta función permite mover el puntero de un archivo de texto hasta el inicio de la siguiente línea, con el fin de continuar la lectura del archivo. Además, la función devuelve la línea actual (antes de mover el puntero) completa (incluyendo el salto de línea) del archivo de texto.

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
El ejemplo anterior permite leer todas las líneas de un archivo de texto y guardarlas dentro de un array.