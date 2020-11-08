# draw_clear

Limpia la superficie de dibujo actual con el color y opacidad dados.

## Sintaxis

  
```gml  
draw_clear_alpha(col, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
col|El color con el cual limpiar la pantalla.|  
alpha|La opacidad con la cual limpiar la pantalla.|  

## Descripción

Esta función permite limpiar la superficie de dibujo actual con el color y opacidad dados. Sólo debe ser utilizada dentro del evento _Draw_ de alguna instancia, o bien para limpiar superficies cuando se necesita dibujar nuevamente en ellas.

## Devuelve

Nada

## Ejemplo

  
```gml  
    
///Evento Draw  
draw_clear_alpha(c_red, 0.5)  
```  
El código anterior limpia la pantalla con el color rojo y opacidad del 50%.