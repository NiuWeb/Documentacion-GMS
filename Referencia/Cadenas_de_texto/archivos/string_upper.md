# string_upper

Convierte las letras minúsculas de una cadena a mayúsculas.

## Sintaxis

  
```gml  
string_upper(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a convertir.|  

## Descripción

Con esta función es posible convertir todas las letras minúsculas de una cadena a mayúsculas.  
  
**NOTA:** Esta función sólo detecta las 26 letras del alfabeto inglés, de la A a la Z.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Hola Mundo";  
mayusculas = string_upper(texto); //Devuelve 'HOLA MUNDO'  
```