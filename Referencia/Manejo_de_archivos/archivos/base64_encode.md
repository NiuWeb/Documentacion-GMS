# base64_encode

Codifica una cadena en formato _base64_.

## Sintaxis

  
```gml  
base64_encode(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a codificar.|  

## Descripción

Esta función permite codificar una cadena en formato _base64_. El formato de codificación _base64_ es utilizado comúmnente para almacenar información sin utilizar caracteres especiales para, por ejemplo, enviarla a través de una URL.  
  
**NOTA:** Cabe mencionar que _base64_ **no** es un formato de encriptación, sino codificación; un texto codificado en _base64_ es fácilmente decodificable.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
codificar = base64_encode("hola"); //Devuelve 'aG9sYQ=='  
```