# string_char_at

Devuelve el caracter ubicado en una posición dada de una cadena.

## Sintaxis

  
```gml  
string_char_at(str, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a revisar.|  
pos|La posición del caracter a obtener.|  

## Descripción

Con esta función, es posible obtener un caracter ubicado en una posición dada de una cadena de texto. La posición 1 equivale al primer caracter de la cadena. Si no se ha encontrado un caracter en la posición dada, o el largor de la cadena es menor a la misma, se devolverá una cadena vacía (`""`).

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Una cadena muy genial";  
  
a = string_char_at(texto, 1); //Devuelve 'U'  
a = string_char_at(texto, 2); //Devuelve 'n'  
a = string_char_at(texto, 4); //Devuelve ' '  
a = string_char_at(texto, 5); //Devuelve 'c'  
a = string_char_at(texto, 2); //Devuelve 'n'  
a = string_char_at(texto, 21); //Devuelve 'l'  
a = string_char_at(texto, 25); //Devuelve ''  
```