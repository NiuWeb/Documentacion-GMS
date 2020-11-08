# ds_stack_write

Escribe la estructura de datos como una cadena de texto.

## Síntaxis

  
```gml  
ds_stack_write(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la pila que se escribirá.|  

## Descripción

Esta función devuelve una cadena de texto que puede ser almacenada o enviada a otra estructura de datos usando la función `ds_stack_read()`.  
  
 _**NOTA:** La cadena de texto no es legible por humanos, es un volcado del contenido de la estructura de datos_.

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
var str;  
ini_open("save.ini");  
str = ds_stack_write(stack);  
ini_write_string("Stacks", "0", str);  
ds_stack_clear(stack);  
ini_close();  
```  
El código anterior abre una archivo ini y luego escribe una cadena de texto que contiene la información almacena en la pila(ds_stack) indexada en la variable "stack". Por último la pila es limpiada y el archivo ini es cerrado.