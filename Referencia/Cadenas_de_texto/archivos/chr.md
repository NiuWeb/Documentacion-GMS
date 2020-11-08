# chr

Devuelve el caracter con el código Unicode dado.

## Sintaxis

  
```gml  
chr(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El código unicode.|  

## Descripción

Esta función devuelve una cadena de texto que contiene el caracter que equivale al código Unicode dado. Este caracter depende de la página de códigos de la fuente de dibujo actual, y si ésta no está definida, se usará la página de códigos por defecto del dispositivo.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
a = chr(65); //Devuelve 'A'  
b = chr(13) + chr(10); //Devuelve un salto de línea  
c = chr(72) + chr(79) + chr(76) + chr(65); //Devuelve 'HOLA'  
```