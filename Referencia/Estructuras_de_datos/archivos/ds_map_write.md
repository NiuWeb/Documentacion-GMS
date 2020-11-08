

# ds_map_write

Esta función escribe los datos de un mapa dentro de una cadena de texto.

## Síntaxis

  
```gml  
ds_map_write(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa|  

## Descripción

Esta función convierte los datos de un mapa especificado a una cadena de texto que puede ser escrita en un archivo *.ini o un archivo de texto *.txt para facilitar su almacenamiento. Esta cadena de texto puede leerse después con la función `ds_map_read()`. _**NOTA:** La cadena de texto generada no es legible para personas, es un volcado de memoria con los datos que contiene._

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
ini_open("map.ini");  
var t_string;  
t_string = ds_map_write(inventory);  
ini_write_string("Saved", "0", t_string);  
ini_close();  
```  
El código anterior apertura un archivo ini, luego inicia una variable temporal, en la cual se guarda la cadena de texto generada con la función `ds_map_write()`; luego se escribe la cadena de texto en el archivo y se cierra.