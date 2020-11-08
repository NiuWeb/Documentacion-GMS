# draw_set_alpha

Establece la opacidad base para las funciones de dibujo.

## Sintaxis

  
```gml  
draw_set_alpha(alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
alpha|La opacidad a establecer. Puede ser un valor entre 0 y 1.|  

## Descripción

Esta función permite establecer la opacidad base para el dibujo de figuras en el juego. sta opacidad puede ser un valor entre 0 y 1, donde 1 es totalmente opaco, y 0 es totalmente transparente.  
  
Esta opacidad afectará a todas las funciones de dibujo que se ejecuten después de esta función, sean _sprites_, _backgrounds_, fuentes, formas básicas e incluso primitivas.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_set_alpha(0.5);  
draw_set_colour(c_black);  
draw_text(x+5, y+5, "LEVEL 1");  
draw_set_alpha(1);  
draw_set_colour(c_white);  
draw_text(x, y, "LEVEL 1");  
```  
El código anterior dibuja un texto en una posición dada con un efecto de sombra creado modificando el color y la opacidad.