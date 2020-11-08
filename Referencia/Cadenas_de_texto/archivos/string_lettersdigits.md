# string_lettersdigits

Devuelve una copia de la cadena dada conteniendo sólo caracteres alfanuméricos.

## Sintaxis

  
```gml  
string_lettersdigits(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a filtrar|  

## Descripción

Con esta función es posible remover todos los caracteres de una cadena dada que no estén clasificados como letras o números.  
  
**NOTA:** Esta función sólo reconoce las 26 letras del alfabeto inglés, de la A a la Z.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Esto_es1_texto que no t1**ene_sen71d0";  
filtro = string_lettersdigits(texto); //Devuelve 'Estoes1textoquenot1enesen71d0'  
```