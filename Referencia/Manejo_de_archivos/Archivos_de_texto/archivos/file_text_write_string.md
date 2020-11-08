# file_text_write_string

Escribe una cadena dentro del archivo de texto dado.

## Sintaxis

  
```gml  
file_text_write_string(fid, str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  
str|La cadena de texto a escribir en el archivo.|  

## Descripción

Esta función permite escribir una cadena de texto dentro de un archivo de texto previamente abierto. Si el archivo ya posee información, ésta será borrada y la cadena será escrita al inicio del archivo, a menos de haberlo abierto mediante `file_text_open_append()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
f = file_text_open_write("info.txt");  
file_text_write_string(f, "Esto es un texto escrito dentro de algún archivo");  
file_text_close(f);  
```  
En el anterior ejemplo, se abre un archivo de texto para su escritura, se escribe en él una cadena de texto y posteriormente se cierra el archivo.