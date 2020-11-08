# string_insert

Inserta una subcadena en la posición dada de la cadena argumentada.

## Sintaxis

  
```gml  
string_insert(substr, str, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
substr|La subcadena a insertar|  
str|La cadena en donde insertar|  
pos|La posición en donde insertar|  

## Descripción

Esta función devuelve una copia de la cadena original, con la subcadena dada insertada en una posición determinada. La posición del primer caracter de una cadena es 1.  
  
**NOTA:** Esta función **no** modifica la cadena original, sólo devuelve una copia modificada.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
a = "Hola,cómo estás?";  
b = string_insert(" Pepito; ¿", a, 6); //Devuelve 'Hola, Pepito; ¿cómo estás?'  
```