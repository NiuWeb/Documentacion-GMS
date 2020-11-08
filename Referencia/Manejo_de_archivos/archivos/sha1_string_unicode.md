# sha1_string_unicode

Devuelve un _Hash SHA-1_ del formato Unicode de la cadena dada.

## Sintaxis

  
```gml  
sha1_string_unicode(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a la cual obtener el Hash SHA-1.|  

## Descripción

SHA-1 es una función criptográfica de Hash diseñada por la Agencia de Seguridad Nacional de los Estados Unidos, y es implementada en muchas aplicaciones de seguridad. Esta función toma la cadena ingresada en formato Unicode (Lo que significa, 16bits por cada caracter) y devuelve un mensaje de 160 bits en formato ASCII, único para la cadena dada.  
  
**NOTA:** Hay dos formatos para la encriptación SHA-1: UTF-8 y Unicode, aunque el más común es el formato Unicode.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
hash = sha1_string_unicode("hola"); //Devuelve 'cd59beba6a60dbc5295c55d780257d6d2dca3031'  
```