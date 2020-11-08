# string_digits

Devuelve una copia de la cadena dada conteniendo sólo números.

## Sintaxis

  
```gml  
string_digits(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a filtrar.|  

## Descripción

Esta función permite obtener sólo los caracteres numéricos que contiene una cadena.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Soy una cadena que contiene el número 2, que es mayor que 1 pero menor a 3.";  
nums = string_digits(texto); //Devuelve '213', como cadena de texto.  
```