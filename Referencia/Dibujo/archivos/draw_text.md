# draw_text

Dibuja un texto en la posición dada.

## Síntaxis

  
```gml  
draw_text(x, y, str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal en donde dibujar el texto.|  
y|La posición vertical en donde dibujar el texto.|  
str|La cadena de texto a dibujar.|  

## Descripción

Esta función permite dibujar cualquier cadena de texto en una posición determinada de la sala. Esta función **sólo admite** como parámetro str cadenas de texto; si se necesita dibujar en pantalla un número real, debe utilizarse la función `string()` o `string_format()` para convertir dicho número a cadena de texto.  
  
Es posible también añadir un signo de almohadilla (`"#"`) para incluír un salto de línea en el texto. Si, por el contrario, se necesita dibujar este caracter en pantalla y no utilizarlo como salto de línea, debe precederse por una barra inclinada inversa, de esta forma: `"Éste es un # sin salto de línea."`.  
  
El color, opcidad y fuente del texto son las definidas por las funciones `draw_set_colour()`, `draw_set_alpha()` y `draw_set_font()`.   
  
**NOTA:** La posición del texto puede verse influenciada por la alineación del mismo, definida por las funciones `draw_set_halign()` y `draw_set_valign()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
var usuario = "Player1";  
var email  = "player1@correo.com";  
draw_text(x, y, "Tu nombre de usuario es: " + usuario + "#Tu correo electrónico es: " + email);  
```