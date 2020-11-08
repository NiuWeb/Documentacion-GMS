# ds_list_write

Escribe la lista en forma de una cadena de texto.

## Sintaxis

  
```gml  
ds_list_write(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a escribir.|  

## Descripción

Con esta función se obtiene una cadena de texto que puede ser almacenada o transferida a otra lista usando la función `ds_list_read()`.  
  
_**Nota:** La cadena de texto obtenida no es legible por humanos, es un volcado del contenido en la estructura de datos (la lista)._

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
var str;  
ini_open("save.ini");  
str = ds_list_write(list);  
ini_write_string("Lists", "0", str);  
ds_list_clear(list);  
ini_close();  
```  
El código anterior abre un archivo .ini y luego escribe una cadena de texto que contiene la información almacenada dentro de la lista(ds_list) indexada en la variable "list". La lista es limpia al final y luego el archivo .ini es cerrado.