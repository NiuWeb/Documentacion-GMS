# file_text_eof

Comprueba si el puntero del archivo dado ha llegado al final del mismo.

## Sintaxis

  
```gml  
file_text_eof(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  

## Descripción

Esta función permite comprobar si se ha alcanzado el final del archivo de texto dado (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
lineas[0] = 0;  
pos = 0;  
  
f = file_text_open_read("archivo.txt");  
while(!file_text_eof(f)) {  
    lineas[pos++] = file_text_read_string(f);  
    file_text_readln(f);  
}  
file_text_close();  
```  
Se abre un archivo de texto para su lectura, y mientras no se haya terminado de leer, se almacenarán las líneas de éste en un array. Posteriormente se cierra el archivo.