# md5_string_unicode

Devuelve un _Hash MD5_ del formato Unicode de la cadena dada.

## Sintaxis

  
```gml  
md5_string_unicode(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a la cual obtener el Hash MD5.|  

## Descripción

En criptografía, MD5 (_Message-Digest algorithm 5_) es una función de hash de 128 bits bastante común, utilizada en diferentes aplicaciones de seguridad. Esta función toma la cadena dada en formato unicode (lo que significa, 16bits por cada caracter) y devuelve el _Hash MD5_ hexadecimal de 32 caracteres, único para la cadena original.  
  
**NOTA:** Hay dos formatos para la encriptación MD5: UTF-8 y Unicode, aunque el más común es el formato Unicode.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
hash = md5_string_unicode("hola"); //Devuelve '6ef03d50ba96fe64a44e8bc0be049d38'  
```