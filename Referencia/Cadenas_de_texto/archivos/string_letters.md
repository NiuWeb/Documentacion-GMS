# string_letters

Devuelve una copia de la cadena dada conteniendo sólo caracteres alfabéticos.

## Sintaxis

  
```gml  
string_letters(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a filtrar|  

## Descripción

Con esta función es posible remover todos los caracteres de una cadena que no estén clasificados como letras.  
  
**NOTA:** Esta función sólo detecta las 26 letras del alfabeto inglés, de la A a la Z.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Elefante+3s = volador*es";  
filtro = string_letters(texto); //Devuelve 'Elefantesvoladores'  
```