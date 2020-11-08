# file_text_read_real

Lee un número real del archivo dado.

## Sintaxis

  
```gml  
file_text_read_real(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  

## Descripción

Esta función permite obtener un número real tomado de la línea en la que se encuentre el puntero del archivo. Si no se encuentra un número real (éste debe aparecer antes de cualquier caracter no numérico), devolverá 0.

## Devuelve

Número real.

## Ejemplo

  
```gml  
numeros[0] = 0;  
pos = 0;  
f = file_text_open_read("archivo.ini");  
while(!file_text_eof(f)) {  
    numeros[pos++] = file_text_read_real(f);  
    file_text_readln();  
}  
file_text_close(f);  
```  
Se abre un archivo de texto para su lectura, se guardan los números reales leídos del archivo en un array, y posteriormente éste se cierra.