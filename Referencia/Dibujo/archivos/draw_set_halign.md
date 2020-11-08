# draw_set_halign

Establece la alineación horizontal del texto.

## Síntaxis

  
```gml  
draw_set_halign(halign);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
halign|La alineación horizontal del texto.|  

## Descripción

Esta función se utiliza para establecer la forma en la que el texto se alinea horizontalmente. Las siguientes constantes son aceptadas:  
  

Constante|Alineación|Valor numérico|  
---|---|---|  
fa_left|![](imagenes/fa_left.png)|0|  
fa_center|![](imagenes/fa_center.png)|1|  
fa_right|![](imagenes/fa_right.png)|2|  

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_set_colour(c_blue);  
draw_set_halign(fa_center);  
draw_set_font(fn_Texto);  
draw_text(x, y - 64, "¡Hola a todos!");  
```  
Se establece el color azul y la fuente `fn_Texto`, y luego se dibuja un texto centrado horizontalmente con estas propiedades.