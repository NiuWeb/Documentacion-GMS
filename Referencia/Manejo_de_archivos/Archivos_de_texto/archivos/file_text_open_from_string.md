# file_text_open_from_string

Crea y abre un archivo temporal, creado de una cadena de texto, para su lectura.

## Sintaxis

  
```gml  
file_text_open_from_string(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena de texto con la cual crear el archivo.|  

## Descripción

Esta función crea un archivo de texto tomando en cuenta la cadena dada, y lo abre para su lectura. Esta función devuelve el identificador del archivo abierto, el cual debe almacenarse para poder realizar posteriores operaciones con él. Cabe mencionar que este archivo es temporal y sólo permite su lectura, además de ser removido de la memoria al momento de cerrarse.

## Devuelve

Número real.

## Ejemplo

  
```gml  
str =  
"Hola mundo,  
soy un simple texto  
que no sirve de nada";  
lineas[0] = 0;  
pos = 0;  
  
f = file_text_open_from_string(str);  
while(!file_text_eof(f)) {  
    lineas[pos++] = file_text_read_string(f);  
    file_text_readln(f);  
}  
file_text_close(f);  
```  
Básicamente, todas las líneas de la cadena de texto almacenada en la variable `str` se almacenan en el array `lineas`.