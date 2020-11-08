# string_width

Devuelve el anchor (en pixeles) de una cadena de texto.

## Sintaxis

  
```gml  
string_width(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a examinar.|  

## Descripción

Esta función devuelve el anchor (en pixeles) de la cadena dada. Este valor depende de la fuente definida actualmente para dibujo.

## Devuelve

Número real.

## Ejemplo

  
```gml  
texto = "Hola mundo!";  
ancho = string_width(texto);  
draw_text(32, 32, texto);  
draw_text(32 + ancho, 32, "Un texto al frente");  
```  
Se dibuja un texto en pantalla en la posición [32,32], y justo en frente de él, se dibuja otro texto.