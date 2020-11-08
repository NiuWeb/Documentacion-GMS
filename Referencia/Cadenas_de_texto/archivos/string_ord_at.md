# string_ord_at

Devuelve el código Unicode del caracter ubicado en la posición dada de una cadena.

## Sintaxis

  
```gml  
string_ord_at(str, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena en donde buscar.|  
pos|La posición en donde buscar.|  

## Descripción

Esta función permite obtener el código Unicode del caracter ubicado en una posición determinada dentro de la cadena. La posición del primer caracter de una cadena es 1. Si no se ha encontrado ningún caracter, o el largor de la cadena es menor a la posición dada, se devolverá una cadena vacía (`""`).

## Devuelve

Número entero.

## Ejemplo

  
```gml  
texto = "HOLA";  
a = string_ord_at(texto, 1); //Devuelve 72  
a = string_ord_at(texto, 4); //Devuelve 65  
```