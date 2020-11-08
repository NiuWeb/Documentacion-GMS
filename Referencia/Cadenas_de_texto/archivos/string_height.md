# string_height

Devuelve la altura (en pixeles) de una cadena de texto.

## Sintaxis

  
```gml  
string_height(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a la cual obtener su altura.|  

## Descripción

Esta función devuelve la altura (en pixeles) de la cadena ingresada. Esta altura depende de la fuente actualmente definida para dibujo.

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = "Texto arriba";  
b = string_height(a);  
draw_text(32, 32, a);  
draw_text(32, 32 + b, "Texto abajo");  
```  
Se dibuja en pantalla (en las coordenadas [32,32]) el texto `"Texto arriba"`, y justo abajo de éste, el texto `"Texto abajo"`.