# clipboard_get_text

Obtiene el contenido copiado en el portapapeles.

## Sintaxis

  
```gml  
clipboard_get_text();  
```  

## Argumentos

Ninguno

## Descripción

Esta función devuelve el contenido copiado en el portapapeles a modo de cadena de texto. Si el portapapeles no tiene contenido, se devolverá una cadena vacía (`""`).

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
a = clipboard_get_text();  
```