# base64_decode

Decodifica una cadena codificada en formato _base64_.

## Sintaxis

  
```gml  
base64_decode(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena codificada a decodificar.|  

## Descripción

Esta función convierte una cadena codificada anteriormente utilizando el formato _base64_ en texto estándar. El formato de codificación _base64_ es utilizado comúmnente para almacenar información sin utilizar caracteres especiales para, por ejemplo, enviarla a través de una URL.  
  
**NOTA:** Cabe mencionar que _base64_ **no** es un formato de encriptación, sino codificación; un texto codificado en _base64_ es fácilmente decodificable.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
decodifica = base64_decode("aG9sYQ=="); //Devuelve hola  
```