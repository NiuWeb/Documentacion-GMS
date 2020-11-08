# file_text_eoln

Comprueba si el puntero del archivo dado ha llegado al final de la línea actual.

## Sintaxis

  
```gml  
file_text_eoln(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  

## Descripción

Esta función comprueba si el puntero del archivo dado ha llegado al final de una línea (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
numeros[0] = 0;  
pos = 0;  
  
f = file_text_open_read("miarchivo.num");  
while(!file_text_eoln(f)) {  
    numeros[pos++] = file_text_read_real(f);  
}  
file_text_close(f);  
```  
En el ejemplo anterior, se realiza la lectura de todos los números reales de la primera línea del archivo, éstos son almacenados dentro de un array, y posteriormente se cierra el archivo.