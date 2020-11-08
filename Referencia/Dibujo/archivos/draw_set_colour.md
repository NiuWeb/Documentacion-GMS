# draw_set_colour

Establece el color base para las funciones de dibujo.

## Sintaxis

  
```gml  
draw_set_colour(col);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
col|El color a establecer para el dibujado.|  

## Descripción

Con esta función puede establecer el color base para el juego. Este valor afectará todas las funciones de dibujado, incluyendo fuentes, primitivas y 3D. Si cualquiera de las funciones de dibujado mencionadas anteriormente tiene su propio color base, este valor será ignorado.

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
El código anterior dibuja un texto en una posición dada con un efecto de sombra creado modificando el color y la transparencia.