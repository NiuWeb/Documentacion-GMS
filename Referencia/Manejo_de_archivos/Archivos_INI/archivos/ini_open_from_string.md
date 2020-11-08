# ini_open_from_string

Abre un archivo ini temporal a partir de la cadena de texto dada.

## Sintaxis

  
```gml  
ini_open_from_string(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena de texto que contiene la información del archivo ini.|  

## Descripción

Esta función crea un archivo ini temporal desde una cadena de texto, para su lectura y escritura. La cadena de texto ingresada debe tener un correcto formato ini (con secciones, saltos de línea y valores). De lo contrario, el archivo ini no se creará correctamente. Cabe mencionar que el archivo ini es temporal y será eliminado al momento de ser cerrado, descartando toda la información almacenada en él. Sin embargo, con la función `ini_close()` se puede obtener el contenido completo del archivo ini.

## Devuelve

Nada.

## Ejemplo

  
```gml  
archivo =  
"[datos]  
monedas=5  
nivel=23";  
  
ini_open_from_string(archivo);  
monedas = ini_read_real("datos", "monedas", 0); //Devuelve 5  
nivel = ini_read_real("datos", "nivel", 1); //Devuelve 23  
ini_close();  
```