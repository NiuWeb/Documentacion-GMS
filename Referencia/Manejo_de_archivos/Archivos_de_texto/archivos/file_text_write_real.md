# file_text_write_real

Escribe un número real en el archivo dado.

## Sintaxis

  
```gml  
file_text_write_real(fid, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  
val|El valor a escribir en el archivo.|  

## Descripción

Esta función permite escribir un número dentro de un archivo de texto previamente abierto. Cabe mencionar que el valor a escribir puede ser un número real, con un punto (`"."`) como separador de la parte decimal. Si el archivo anteriormente contiene información, ésta será borrada y el valor nuevo se escribirá al inicio del archivo, a excepción de haberlo abierto mediante la función `file_text_open_append()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
valores[0] = 5;  
valores[1] = 3;  
valores[2] = 4.5;  
  
f = file_text_open_write("Valores.txt");  
for(i = 0; i < array_length_1d(valores); i++) {  
    file_text_write_real(f, valores[i]);  
    file_text_writeln(f);  
}  
file_text_close(f);  
```  
Se abre un archivo de texto para su escritura, se escriben en él los valores numéricos almacenados en un array, y posteriormente se cierra el archivo.