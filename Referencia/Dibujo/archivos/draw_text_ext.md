# draw_text_ext

Dibuja un texto en la posición dada con propiedades personalizadas.

## Síntaxis

  
```gml  
draw_text_ext(x, y, str, sep, w);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal en donde dibujar el texto.|  
y|La posición vertical en donde dibujar el texto.|  
str|La cadena de texto a dibujar.|  
sep|La separación vertical entre las líneas de texto.|  
w|El anchor máximo en pixeles antes de un salto de línea.|  

## Descripción

Esta función es muy similar a `draw_text()`, con la diferencia de que es posible establecer el espacio que habrá entre cada línea de texto y limitar el anchor (en pixeles) que tendrá la cadena en cada línea, y cuando éste límite es superado, _GameMaker: Studio_ moverá automáticamente el texto sobrante a la siguiente línea. Si se le da el valor de -1 al argumento sep, la separación del texto será la misma de la fuente que se esté usando.

## Devuelve

Nada.

## Ejemplo

  
```gml  
var usuario = "Player1";  
var email  = "player1@correo.com";  
draw_text(x, y, "Tu nombre de usuario es: " + usuario + "#Tu correo electrónico es: " + email, 16, 320);  
```