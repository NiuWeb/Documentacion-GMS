# string_lower

Convierte las letras mayúsculas de una cadena a minúsculas.

## Sintaxis

  
```gml  
string_lower(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a filtrar|  

## Descripción

Esta función devuelve una copia de la cadena dada con todas las letras minúsculas.  
  
**NOTA:** Esta función sólo detecta las 26 letras del alfabeto inglés, de la A a la Z.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "uN tEXto coN MUchAs MAYuscuLAS y MInuscULas.";  
minusculas = string_lower(texto); //Devuelve 'un texto con muchas mayusculas y minusculas'  
```