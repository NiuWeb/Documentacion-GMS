# sha1_string_utf8

Devuelve un _Hash SHA-1_ del formato UTF-8 de la cadena dada.

## Sintaxis

  
```gml  
sha1_string_utf8(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a la cual obtener el Hash SHA-1.|  

## Descripción

SHA-1 es una función criptográfica de Hash diseñada por la Agencia de Seguridad Nacional de los Estados Unidos, y es implementada en muchas aplicaciones de seguridad. Esta función toma la cadena ingresada en formato UTF-8 (lo que significa una cantidad de bytes variable por cada caracter) y devuelve un mensaje de 160 bits en formato ASCII.  
  
**NOTA:** Hay dos formatos para la encriptación SHA-1: UTF-8 y Unicode, aunque el más común es el formato Unicode.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
hash = sha1_string_utf8("hola"); //Devuelve '99800b85d3383e3a2fb45eb7d0066a4879a9dad0'  
```