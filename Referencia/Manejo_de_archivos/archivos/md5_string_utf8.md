# md5_string_utf8

Devuelve un _Hash MD5_ del formato UTF-8 de la cadena dada.

## Sintaxis

  
```gml  
md5_string_utf8(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a la cual obtener el Hash MD5.|  

## Descripción

En criptografía, MD5 (_Message-Digest algorithm 5_) es una función de hash de 128 bits bastante común, utilizada en diferentes aplicaciones de seguridad. Esta función toma la cadena ingresada en formato UTF-8 (lo que significa, un número variable de bytes por caracter) y devuelve el Hash MD5 hexadecimal de 32 caracteres, único para la cadena original.  
  
**NOTA:** Hay dos formatos para la encriptación MD5: UTF-8 y Unicode, aunque el más común es el formato Unicode.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
hash = md5_string_utf8("hola"); //Devuelve '4d186321c1a7f0f354b297e8914ab240'  
```