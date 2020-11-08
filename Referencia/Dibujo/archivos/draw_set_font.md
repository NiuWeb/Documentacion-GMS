# draw_set_font

Establece la fuente que se usará para dibujar el texto.

## Síntaxis

  
```gml  
draw_set_font(font);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
font|El índice de la fuente a establecer.|  

## Descripción

Esta función establece la fuente que se usará para dibujar el texto. El parámetro font debe ser una constante que represente un recurso de fuente incluído en el proyecto, o bien un identificador de fuente externa devuelto por `font_add()` y/o `font_add_sprite()`. También es posible utilizar -1 como parámetro para establecer la fuente por defecto: Arial de 12pt.  
  
**NOTA:** Hasta que no se cambie nuevamente, todos los textos en el juego se dibujarán con la fuente que esta función establezca. Es decir, es de uso global.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_colour(c_blue);  
draw_set_font(fn_Texto);  
draw_text(x, y - 64, "¡Hola a todos!");  
```  
Se establece el color azul y la fuente `fn_Texto`, y luego se dibuja un texto con estas propiedades.