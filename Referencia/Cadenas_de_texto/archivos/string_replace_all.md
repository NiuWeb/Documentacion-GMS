# string_replace_all

Reemplaza todas las coincidencias de una subcadena en una cadena por otra.

## Sintaxis

  
```gml  
string_replace_all(str, substr, newstr);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena en donde buscar.|  
substr|La cadena a reemplazar.|  
newstr|La cadena por la cual reemplazar.|  

## Descripción

Esta función permite reemplzar todas las coincidencias de una subcadena dentro de una cadena por otra.  
  
**NOTA:** Esta función **no** modifica la cadena original, sólo devuelve una copia modificada de la misma.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Hola mundo";  
nuevo = string_replace_all(texto, "mundo", "Pepito"); //Devuelve 'Hola Pepito'  
  
texto = "El mundo es un mundo mejor que cualquier otro mundo";  
nuevo = string_replace_all(texto, "mundo", "tren"); //Devuelve 'El tren es un tren mejor que cualquier otro tren'  
```